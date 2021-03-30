---
title: Encontre aplicações em falta na lâmina de registo de aplicações
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
- "9004352"
- "9654"
ms.openlocfilehash: 00b5821e2edad8b60ff60b1f85264d81c72277e4
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/23/2021
ms.locfileid: "51405217"
---
# <a name="find-missing-applications-on-app-registration-blade"></a>Encontre aplicações em falta na lâmina de registo de aplicações

1. Não é possível encontrar aplicações no portal de Registo de Aplicações.

    Se uma aplicação for uma aplicação multi-inquilino e foi registada noutro inquilino, não será exibida sob a lâmina de Registo de Aplicações. No entanto, poderá encontrá-la sob a lâmina de Aplicações empresariais uma vez que tenha sido acedida (depois de consentida) e o principal de serviço foi criado no seu inquilino. Para mais informações, consulte [os principais de serviços & apps em Azure AD - plataforma de identidade da Microsoft](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals).
2. Não é possível ver aplicações na lâmina de Registo de Aplicações, mesmo que seja um administrador.

    Certifique-se de que está no diretório certo no portal Azure.
3. A minha aplicação não está listada na lâmina de Aplicações da Empresa, mas aparece quando consulta o comando PowerShell.

    Por vezes, depois de eliminar a aplicação do portal Azure, não aparece no portal, mas pode não ter sido completamente eliminada. Para mais informações, consulte:
    - Pode recuperar a lista de aplicações previamente eliminadas e ver se a aplicação aparece na lista utilizando o comando Powershell: **Get-AzureADDeletedApplication**. Para saber mais, consulte [Get-AzureADDeletedApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureaddeletedapplication).
    - Se quiser remover completamente a aplicação, pode experimentar o seguinte em PowerShell: **Remove-AzureADApplication -ObjectId**. Para saber mais, consulte [Remove-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplication).
    - Em alternativa, pode tentar restaurar a aplicação eliminada utilizando o seguinte comando Powershell: **Restaurar AzureADDeletedApplication -ObjectId**. Para saber mais, consulte [Restore-AzureADDeletedApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).
4. Não consigo encontrar a lista de todas as aplicações de empresa pré-instaladas no meu novo inquilino da Azure.

    Não existem aplicações empresariais pré-instaladas no Azure AD por padrão. Tem de adicioná-lo manualmente a partir da opção "Nova aplicação", navegando-a na galeria AZure AD ou adicionando uma aplicação não-galeria. Para saber mais, consulte [Quickstart: Adicione uma aplicação ao seu inquilino Azure Ative Directory (Azure AD).](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal)
    Se for um administrador global, pode aceder facilmente às suas aplicações utilizando o [Launcher da aplicação Microsoft 365.](https://docs.microsoft.com/microsoft-365/admin/manage/customize-the-app-launcher)
5. Incapaz de encontrar as minhas aplicações do portal My Apps.

    Certifique-se de que as aplicações não estão escondidas na página de recolha das Minhas Apps. Para saber mais, consulte [Coleções (pré-visualização) no portal My Apps - Azure AD](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-user-collections).
6. Para iniciar aplicações a partir do portal My Apps, consulte [localizar & utilizar aplicações no portal My Apps - Azure AD](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-end-user-access).
7. A aplicação Do Office 365 Mover não aparece na lâmina das aplicações da Empresa após a instalação.

    A aplicação "Office 365 Mover" é uma aplicação multitenante que não precisa de ser adicionada à AAD utilizando a secção de Aplicações de Galeria ao abrigo do Registo de Aplicações da Empresa. Para aceder à aplicação Do Office 365 Mover, basta iniciar s-in na aplicação e pedir o consentimento do utilizador para as permissões. Assim que o utilizador fornecer o consentimento, esta aplicação será automaticamente adicionada ao inquilino com o id de e-mail que fez login.

    Após a assinatura da aplicação, deverá ser possível encontrar a entrada desta aplicação sob a lâmina das Aplicações empresariais em AAD. Você precisa procurar por essa aplicação digitando o nome completo, ou seja, "Office 365 Mover" ou simplesmente pesquisar "office" e deve listar a aplicação. Para saber mais, consulte [o Office 365 Mover diz que já está instalado, mas não está listado na galeria de aplicações da Empresa.](https://docs.microsoft.com/answers/questions/30186/office-365-mover-says-its-already-installed-but-it.html)
8. [Quickstart: Veja a lista de aplicações que estão a usar o seu inquilino Azure Ative (Azure AD) para gestão de identidade](https://docs.microsoft.com/azure/active-directory/manage-apps/view-applications-portal) mostra-lhe como visualizar as aplicações, também conhecidas como apps, que já estão configuradas para usar o seu inquilino Azure AD como seu Fornecedor de Identidade (IdP).
9. [Resolver problemas comuns adicionando ou removendo uma aplicação para Azure Ative Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-adding-apps) ajuda-o a entender os problemas comuns que as pessoas enfrentam ao ver aplicações no Azure Ative Directory.
