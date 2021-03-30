---
title: Problemas do Proprietário do Registo de Aplicações
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
ms.openlocfilehash: 9dc3b1d54bb263d5e53e02a4e4dadc8cf3c1e400
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/23/2021
ms.locfileid: "51405317"
---
# <a name="app-registration-owner-issues"></a>Problemas do Proprietário do Registo de Aplicações

Seguem-se os métodos disponíveis para adicionar os principais como proprietários para registos de aplicações:

- Usando módulo Ad PowerShell -

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    Referência: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)
- Usando O Azure CLI - `az ad app owner add`

    Referência: [az ad app proprietário](https://docs.microsoft.com/cli/azure/ad/app/owner)
- Usando o Ms Graph -

    Referência: [Adicionar proprietário - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)
- Utilização do Portal AD Azure - Navegue para [portal.azure.com](https://portal.azure.com/) > diretório Azure Ative > Registo de Aplicações > Selecione a sua aplicação > Proprietários > Adicionar Proprietários

**Não é possível ver a sua aplicação na lâmina de Registos de Aplicações, mesmo que seja o proprietário dessa aplicação?**

O proprietário de uma aplicação não é um papel administrativo. Se a definição Restringir o [acesso ao portal de administração AD do Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) está ativado, apenas a administração poderá visualizar as aplicações no portal de Registo de Aplicações. Para que um proprietário possa visualizar as aplicações, desative esta definição (Defina isto para NO) ou atribua função de administração ao proprietário apenas para a aplicação específica. No entanto, você vai precisar de uma licença Azure AD Premium P2 e ativar [a Gestão de Identidade Privilegiada.](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)
