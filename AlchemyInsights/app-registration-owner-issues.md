---
title: Problemas com o Proprietário do Registo de Aplicações
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
- "9655"
ms.openlocfilehash: cd7533f09ed8361e134b81979532cdebbf49971c54553a0172c7527f30e319bb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951144"
---
# <a name="app-registration-owner-issues"></a>Problemas com o Proprietário do Registo de Aplicações

Seguem-se os métodos disponíveis para adicionar principais como proprietários de registos de aplicações:

- Utilizar o Módulo PowerShell do Azure AD -

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    Referência: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)
- Utilizar o Azure CLI - `az ad app owner add`

    Referência: [proprietário da aplicação Az AD](https://docs.microsoft.com/cli/azure/ad/app/owner)
- Utilizar ms Graph -

    Referência: [Adicionar proprietário - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)
- Utilizar o Portal do Azure AD – navegue para [o portal.azure.com](https://portal.azure.com/) > Registo de Aplicações do > Active Directory > > Selecione a sua aplicação > Proprietários > Adicionar Proprietários

**Não é possível ver a sua aplicação no blade Registrations (Registos de Aplicações) mesmo que seja o proprietário da aplicação?**

O proprietário de uma aplicação não é uma função administrativa. Se a definição Restringir o acesso ao portal de administração do [Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) estiver ativada, apenas o administrador poderá ver as aplicações no portal de Registo de Aplicações. Para um proprietário poder ver as aplicações, desativar esta definição (Definir isto para NÃO) ou atribuir função de administrador ao proprietário apenas para a aplicação específica. No entanto, para tal, precisará de uma licença Azure AD Premium P2 ativar [o Privileged Identity Management.](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)
