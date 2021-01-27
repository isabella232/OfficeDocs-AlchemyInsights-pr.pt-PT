---
title: Eliminar ou restaurar aplicações
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004335"
- "7737"
ms.openlocfilehash: 4df9a98644f6bc7a30f9009719c5198db591afc9
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014907"
---
# <a name="delete-or-restore-applications"></a>Eliminar ou restaurar aplicações

**Para eliminar uma aplicação do seu inquilino AZure AD:**

1. No **portal AD AZure,** selecione **aplicações Enterprise**. Em seguida, encontre e selecione a aplicação que pretende eliminar.
2. Na secção **Gerir** no painel esquerdo, selecione **Propriedades**.
3. **Selecione Eliminar**, e em seguida, selecione **Sim** para confirmar que deseja eliminar a aplicação do seu inquilino AD Azure.

Para obter mais informações sobre como eliminar uma aplicação, consulte [Quickstart: Elimine uma aplicação do seu inquilino Azure Ative Directory (Azure AD).](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant)

Em PowerShell, o [cmdlet Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) remove as configurações de procuração de aplicação de uma aplicação específica no Diretório Ativo Azure, e pode eliminar completamente a aplicação se especificada.

Pode **restaurar uma aplicação eliminada** utilizando o PowerShell. Uma vez identificada a aplicação que pretende restaurar, pode restaurá-la utilizando [o Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).
