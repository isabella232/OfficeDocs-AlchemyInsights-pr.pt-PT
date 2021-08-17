---
title: Obter uma lista de Aplicações Empresariais
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004342"
- "9837"
ms.openlocfilehash: 99e4f7e676610103355736ce847930c6c5d2d7532c4756ac4551a8d9b3020176
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54116739"
---
# <a name="get-a-list-of-enterprise-applications"></a>Obter uma lista de Aplicações Empresariais

1. Para obter uma lista de aplicações empresariais (todas as **aplicações** ou filtradas pelo Nome a apresentar, ID, URIs de Identificador, etc.) através do comando PowerShell, consulte [Get-AzureADApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication)
2. Para obter uma lista dos objetos principais do serviço (todos os objetos ou filtrados pelo ID) através do comando PowerShell, consulte [Get-AzureADServicePrincipal (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal)
3. Se quiser obter uma **lista de aplicações configuradas por SAML,** os seguintes scripts do PowerShell poderão ajudá-lo:

    Cada Aplicação pode ser uma aplicação OAuth ou uma aplicação SAML (tanto a galeria como as aplicações que não sejam da galeria) teriam dois objetos criados no AAD quando o registo ocorre. Um é denominado Objeto Application e o outro é o objeto Principal do Serviço. Quando deteta as propriedades de um Objeto Principal de Serviço através do PowerShell, veria que todas as aplicações têm um determinado número de Etiquetas associadas ao mesmo do tipo:

    - As aplicações OAuth teriam uma etiqueta chamada "**WindowsAzureActiveDirectoryIntegratedApp**"
    - Aplicações SAML da Galeria teria uma etiqueta denominada "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"
    - As Aplicações SAML que não são da Galeria teriam uma etiqueta denominada "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"

    Por isso, pode utilizar estas etiquetas e descobrir que tipo de aplicação é. A etiqueta "**WindowsAzureActiveDirectoryIntegratedApp**" é comum a todos os tipos de aplicações. Pode utilizar o seguinte snipet para listar todas as aplicações SAML (galeria e não galeria):

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    Para obter mais informações, consulte [Identificar aplicações com saml no Azure AD.](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html)

4. **Encontrar e listar apenas** aplicações Web: utilize o comando abaixo para obter todas as aplicações do Azure AD com o tipo de aplicação "Aplicação Web/API"

    Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -ne $true } | FT
5. **Encontre e liste apenas aplicações nativas:** execute o seguinte comando para obter todas as aplicações de cliente nativa (computador/dispositivo móvel).

    Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -eq $true } | FT
6. Exportar todos os Detalhes da **Aplicação Azure AD** Registados para CSV: o comando abaixo exporta todas as aplicações do Azure AD com detalhes necessários para o ficheiro csv:

    - Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |
    - Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Codificação UTF8

7. **Precisa de exportar uma lista de aplicações do Azure nãoutilizadas** – relatório de auditoria

    O Azure AD pode mostrar registos de aplicações durante apenas 30 dias, desde que tenha Azure AD Premium licença.
    Tem duas opções para manter os dados durante mais de 30 dias. Pode utilizar as APIs de Relatórios do [Azure AD](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) para obter os dados através de programação e armazená-los numa base de dados. Em alternativa, pode integrar os registos de auditoria num sistema SIEM de terceiros.

    Também pode transferir a lista de aplicações para todas as aplicações e aplicações propriedade no Azure Active directory>Registos da Aplicação>Transferir>Todas as aplicações/Aplicações propriedades.

    Para obter uma lista das aplicações através do MS Graph, consulte Aplicações de lista [– Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) e tipo de recurso de aplicação [– Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).
