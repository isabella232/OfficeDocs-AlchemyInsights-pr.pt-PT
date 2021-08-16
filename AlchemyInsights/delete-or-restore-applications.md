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
ms.openlocfilehash: 0c7be98650ca87f36b66f0bb38fb665fc81525b7f3410da14b99fb67468c1e73
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54102582"
---
# <a name="delete-or-restore-applications"></a>Eliminar ou restaurar aplicações

**Para eliminar uma aplicação do seu inquilino do Azure AD:**

1. No portal do **Azure AD , selecione** **Aplicações empresariais**. Em seguida, localcione e selecione a aplicação que pretende eliminar.
2. Na secção **Gerir** no painel esquerdo, selecione **Propriedades**.
3. **Selecione Eliminar e,** em seguida, **selecione** Sim para confirmar que pretende eliminar a aplicação do seu inquilino do Azure AD.

Para obter mais informações sobre como eliminar uma aplicação, consulte Guia de Utilização: Eliminar uma aplicação do seu inquilino [do Azure Active Directory (Azure AD).](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant)

No PowerShell, o cmdlet [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) remove configurações do Application Proxy de uma aplicação específica no Azure Active Directory e pode eliminar a aplicação completamente, se especificado.

Pode **restaurar uma aplicação eliminada** com o PowerShell. Assim que a aplicação que pretende restaurar tiver sido identificada, pode restaurá-la através de [Restore-AzureADDeletedApplication.](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)
