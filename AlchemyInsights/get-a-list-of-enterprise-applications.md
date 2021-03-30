---
title: Obtenha uma lista de Aplicações empresariais
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
ms.openlocfilehash: f5c1a77e415d4bbaa5718a6668af95934db7e5ae
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/26/2021
ms.locfileid: "51405516"
---
# <a name="get-a-list-of-enterprise-applications"></a>Obtenha uma lista de Aplicações empresariais

1. Para **obter uma lista de aplicações empresariais** (todas as aplicações ou filtradas pelo nome display, ID, Identifier URIs, etc.) através do comando Powershell, consulte [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).
2. Para obter uma lista de objetos principais de serviço (todos os objetos ou filtrados por ID) através do comando Powershell, consulte [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).
3. Se quiser **obter uma lista de aplicações configuradas pela SAML, seguir scripts PowerShell** pode ajudá-lo:

    Cada Aplicação seja uma aplicação OAuth ou uma aplicação SAML (tanto de galeria como de aplicações não-galeria) teriam dois objetos criados no AAD quando o seu registo acontecesse. Um é chamado de Objeto de Aplicação e o outro é o objeto principal de serviço. Quando despeja as propriedades de um Objeto Principal de Serviço usando o PowerShell, descobriria que cada aplicação tem um certo número de Tags associadas a ele como:

    - As aplicações OAuth teriam uma etiqueta chamada "**WindowsAzureActiveDirectoryIntegratedApp**"
    - A Gallery SAML Apps teria uma etiqueta chamada "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"
    - Não Galeria SAML Apps teria uma etiqueta chamada "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"

    Assim, você pode usar estas tags e descobrir que tipo de app é. A tag "**WindowsAzureActiveDirectoryIntegratedApp**" é comum a todos os tipos de aplicações. Você pode usar o corte seguinte para listar todas as aplicações SAML (tanto galeria como não-galeria):

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    Para obter mais informações, consulte [identificar aplicações ativadas pela SAML em Azure AD](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html).

4. **Localizar e listar apenas aplicações Web**: Use o comando abaixo para obter todas as aplicações AD Azure com o tipo de aplicação "Web app/API"

    Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -ne $true } | FT
5. **Encontre e liste apenas aplicações nativas**: Executar o seguinte comando para obter todas as aplicações do cliente nativo (desktop/dispositivo móvel).

    Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -eq $true } | FT
6. **Exportar todos os detalhes da aplicação Azure AD registados para o CSV**: O comando abaixo exporta todas as aplicações AD AZure com detalhes necessários para o ficheiro CSV:

    - Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient,AvailableToOtherTenants, HomePage, LogoutUrl |
    - Export-Csv "C:\AzureADApps.csv" - NoTypeInformation -Codificação UTF8

7. **Necessidade de exportar uma lista de aplicações Azure não usused** – Relatório de auditoria

    O Azure AD pode apresentar registos de candidaturas por apenas 30 dias desde que tenha licença Azure AD Premium.
    Tem duas opções para reter os dados por mais de 30 dias. Pode utilizar as [APIs de relato de Ad Azure](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) para recuperar os dados programáticamente e armazená-los numa base de dados. Em alternativa, pode integrar registos de auditoria num sistema SIEM de terceiros.

    Também pode descarregar a lista de aplicações para todas as aplicações e aplicações de propriedade sob o diretório Azure Ative>Registos de Aplicações>Descarregar>todas as aplicações/aplicações próprias.

    Para obter uma lista de aplicações através do MS Graph, consulte [as aplicações List - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) e [tipo de recurso de aplicação - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).
