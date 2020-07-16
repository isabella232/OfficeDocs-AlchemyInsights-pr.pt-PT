---
title: Questões de licenciamento yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 6d9b2126dc1ed90968738ddb2e249dce9857f1db
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148317"
---
# <a name="yammer-licensing-issues"></a><span data-ttu-id="3c515-102">Questões de licenciamento yammer</span><span class="sxs-lookup"><span data-stu-id="3c515-102">Yammer licensing issues</span></span>

<span data-ttu-id="3c515-103">Todos os utilizadores devem ter uma licença para usar o serviço Yammer Enterprise, mas por padrão a Yammer não requer que os utilizadores tenham uma licença para aceder ao serviço.</span><span class="sxs-lookup"><span data-stu-id="3c515-103">All users must have a license to use the Yammer Enterprise service, but by default Yammer does not require that users have a license to access the service.</span></span> <span data-ttu-id="3c515-104">Quando um administrador altera a definição para bloquear utilizadores da Microsoft 365 sem licenças Yammer, os utilizadores não atribuídos a uma licença Yammer Enterprise não podem aceder ao serviço Yammer.</span><span class="sxs-lookup"><span data-stu-id="3c515-104">When an administrator changes the setting to block Microsoft 365 users without Yammer licenses, users not assigned a Yammer Enterprise license can't access the Yammer service.</span></span> <span data-ttu-id="3c515-105">Para mais informações, consulte [as licenças de utilizador da Manage Yammer no Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="3c515-105">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span></span> 

<span data-ttu-id="3c515-106">Quando as licenças são removidas dos utilizadores, o azulejo Yammer já não é apresentado, e outros serviços podem usar a remoção da licença para ocultar funcionalidades.</span><span class="sxs-lookup"><span data-stu-id="3c515-106">When licenses are removed from users, the Yammer tile is no longer displayed, and other services can use license removal to hide features.</span></span> <span data-ttu-id="3c515-107">Noutros casos, as características ainda podem aparecer, mas requerem a atribuição de licenças para operar.</span><span class="sxs-lookup"><span data-stu-id="3c515-107">In other cases, features can still appear but require licence assignment to operate.</span></span>  

<span data-ttu-id="3c515-108">**A licença não está a ser atualizada para o utilizador**</span><span class="sxs-lookup"><span data-stu-id="3c515-108">**License is not getting updated for the user**</span></span>  

<span data-ttu-id="3c515-109">Ocasionalmente, um utilizador é atribuído a uma licença, mas ainda não consegue aceder a Yammer.</span><span class="sxs-lookup"><span data-stu-id="3c515-109">Occasionally, a user is assigned a license but is still unable to access Yammer.</span></span> <span data-ttu-id="3c515-110">Os atrasos são mais prováveis de ocorrer quando uma atribuição de licença em massa está em andamento.</span><span class="sxs-lookup"><span data-stu-id="3c515-110">Delays are more likely to occur when a mass license assignment is in progress.</span></span> <span data-ttu-id="3c515-111">Os utilizadores de Yammer podem não ser atualizados na mesma ordem que as licenças são alteradas em Azure AD porque o sistema funciona assíncronamente.</span><span class="sxs-lookup"><span data-stu-id="3c515-111">Yammer users might not be updated in the same order as licenses are changed in Azure AD because the system runs asynchronously.</span></span> <span data-ttu-id="3c515-112">Aguarde até 24 horas antes de abrir um caso de apoio para reportar problemas de sincronização de licenças.</span><span class="sxs-lookup"><span data-stu-id="3c515-112">Wait up to 24 hours before opening a support case to report license sync issues.</span></span>  

<span data-ttu-id="3c515-113">**Atribuição de licença a granel**</span><span class="sxs-lookup"><span data-stu-id="3c515-113">**Bulk licence assignment**</span></span>  

<span data-ttu-id="3c515-114">As licenças podem ser atribuídas através do centro de administração ou da scripting PowerShell.</span><span class="sxs-lookup"><span data-stu-id="3c515-114">Licenses can be assigned through the admin center or PowerShell scripting.</span></span> <span data-ttu-id="3c515-115">Para obter mais informações, consulte [atribuir licenças aos utilizadores](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) e [atribuir licenças às contas dos utilizadores com o Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span><span class="sxs-lookup"><span data-stu-id="3c515-115">For more info, see [Assign licenses to users](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) and [Assign licenses to user accounts with Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span></span> 

<span data-ttu-id="3c515-116">O Microsoft Support não presta assistência na criação de scripts, mas a documentação sobre a atribuição da licença Yammer está disponível.</span><span class="sxs-lookup"><span data-stu-id="3c515-116">Microsoft Support does not provide assistance with creating scripts, but documentation on Yammer license assignment is available.</span></span> <span data-ttu-id="3c515-117">Para obter mais informações, consulte [as licenças Manage Yammer utilizando o Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span><span class="sxs-lookup"><span data-stu-id="3c515-117">For more info, see [Manage Yammer licenses by using Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span></span>