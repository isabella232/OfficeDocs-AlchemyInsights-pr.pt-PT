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
# <a name="delete-or-restore-applications"></a><span data-ttu-id="e83f4-102">Eliminar ou restaurar aplicações</span><span class="sxs-lookup"><span data-stu-id="e83f4-102">Delete or restore applications</span></span>

<span data-ttu-id="e83f4-103">**Para eliminar uma aplicação do seu inquilino AZure AD:**</span><span class="sxs-lookup"><span data-stu-id="e83f4-103">**To delete an application from your Azure AD tenant**:</span></span>

1. <span data-ttu-id="e83f4-104">No **portal AD AZure,** selecione **aplicações Enterprise**.</span><span class="sxs-lookup"><span data-stu-id="e83f4-104">In the **Azure AD portal**, select **Enterprise applications**.</span></span> <span data-ttu-id="e83f4-105">Em seguida, encontre e selecione a aplicação que pretende eliminar.</span><span class="sxs-lookup"><span data-stu-id="e83f4-105">Then find and select the application you want to delete.</span></span>
2. <span data-ttu-id="e83f4-106">Na secção **Gerir** no painel esquerdo, selecione **Propriedades**.</span><span class="sxs-lookup"><span data-stu-id="e83f4-106">In the **Manage** section in the left pane, select **Properties**.</span></span>
3. <span data-ttu-id="e83f4-107">**Selecione Eliminar**, e em seguida, selecione **Sim** para confirmar que deseja eliminar a aplicação do seu inquilino AD Azure.</span><span class="sxs-lookup"><span data-stu-id="e83f4-107">Select **Delete**, and then select **Yes** to confirm you want to delete the app from your Azure AD tenant.</span></span>

<span data-ttu-id="e83f4-108">Para obter mais informações sobre como eliminar uma aplicação, consulte [Quickstart: Elimine uma aplicação do seu inquilino Azure Ative Directory (Azure AD).](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant)</span><span class="sxs-lookup"><span data-stu-id="e83f4-108">For more information on how to delete an app, see [Quickstart: Delete an application from your Azure Active Directory (Azure AD) tenant](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).</span></span>

<span data-ttu-id="e83f4-109">Em PowerShell, o [cmdlet Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) remove as configurações de procuração de aplicação de uma aplicação específica no Diretório Ativo Azure, e pode eliminar completamente a aplicação se especificada.</span><span class="sxs-lookup"><span data-stu-id="e83f4-109">In PowerShell, the [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) cmdlet removes Application Proxy configurations from a specific application in Azure Active Directory, and can delete the application completely if specified.</span></span>

<span data-ttu-id="e83f4-110">Pode **restaurar uma aplicação eliminada** utilizando o PowerShell.</span><span class="sxs-lookup"><span data-stu-id="e83f4-110">You can **restore a deleted application** using PowerShell.</span></span> <span data-ttu-id="e83f4-111">Uma vez identificada a aplicação que pretende restaurar, pode restaurá-la utilizando [o Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).</span><span class="sxs-lookup"><span data-stu-id="e83f4-111">Once the application you want to restore has been identified, you can restore it using [Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).</span></span>
