---
title: Questões de licenciamento yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: f0a7625c7b77860e5ba0e29f2df47101749aace3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47657287"
---
# <a name="yammer-licensing-issues"></a><span data-ttu-id="a0b25-102">Questões de licenciamento yammer</span><span class="sxs-lookup"><span data-stu-id="a0b25-102">Yammer licensing issues</span></span>

<span data-ttu-id="a0b25-103">Todos os utilizadores devem ter uma licença para usar o serviço Yammer Enterprise, mas por padrão a Yammer não requer que os utilizadores tenham uma licença para aceder ao serviço.</span><span class="sxs-lookup"><span data-stu-id="a0b25-103">All users must have a license to use the Yammer Enterprise service, but by default Yammer does not require that users have a license to access the service.</span></span> <span data-ttu-id="a0b25-104">Quando um administrador altera a definição para bloquear utilizadores da Microsoft 365 sem licenças Yammer, os utilizadores não atribuídos a uma licença Yammer Enterprise não podem aceder ao serviço Yammer.</span><span class="sxs-lookup"><span data-stu-id="a0b25-104">When an administrator changes the setting to block Microsoft 365 users without Yammer licenses, users not assigned a Yammer Enterprise license can't access the Yammer service.</span></span> <span data-ttu-id="a0b25-105">Para mais informações, consulte [as licenças de utilizador da Manage Yammer no Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="a0b25-105">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span></span> 

<span data-ttu-id="a0b25-106">Quando as licenças são removidas dos utilizadores, o azulejo Yammer já não é apresentado, e outros serviços podem usar a remoção da licença para ocultar funcionalidades.</span><span class="sxs-lookup"><span data-stu-id="a0b25-106">When licenses are removed from users, the Yammer tile is no longer displayed, and other services can use license removal to hide features.</span></span> <span data-ttu-id="a0b25-107">Noutros casos, as características ainda podem aparecer, mas requerem a atribuição de licenças para operar.</span><span class="sxs-lookup"><span data-stu-id="a0b25-107">In other cases, features can still appear but require licence assignment to operate.</span></span>  

<span data-ttu-id="a0b25-108">**A licença não está a ser atualizada para o utilizador**</span><span class="sxs-lookup"><span data-stu-id="a0b25-108">**License is not getting updated for the user**</span></span>  

<span data-ttu-id="a0b25-109">Ocasionalmente, um utilizador é atribuído a uma licença, mas ainda não consegue aceder a Yammer.</span><span class="sxs-lookup"><span data-stu-id="a0b25-109">Occasionally, a user is assigned a license but is still unable to access Yammer.</span></span> <span data-ttu-id="a0b25-110">Os atrasos são mais prováveis de ocorrer quando uma atribuição de licença em massa está em andamento.</span><span class="sxs-lookup"><span data-stu-id="a0b25-110">Delays are more likely to occur when a mass license assignment is in progress.</span></span> <span data-ttu-id="a0b25-111">Os utilizadores de Yammer podem não ser atualizados na mesma ordem que as licenças são alteradas em Azure AD porque o sistema funciona assíncronamente.</span><span class="sxs-lookup"><span data-stu-id="a0b25-111">Yammer users might not be updated in the same order as licenses are changed in Azure AD because the system runs asynchronously.</span></span> <span data-ttu-id="a0b25-112">Aguarde até 24 horas antes de abrir um caso de apoio para reportar problemas de sincronização de licenças.</span><span class="sxs-lookup"><span data-stu-id="a0b25-112">Wait up to 24 hours before opening a support case to report license sync issues.</span></span>  

<span data-ttu-id="a0b25-113">**Atribuição de licença a granel**</span><span class="sxs-lookup"><span data-stu-id="a0b25-113">**Bulk licence assignment**</span></span>  

<span data-ttu-id="a0b25-114">As licenças podem ser atribuídas através do centro de administração ou da scripting PowerShell.</span><span class="sxs-lookup"><span data-stu-id="a0b25-114">Licenses can be assigned through the admin center or PowerShell scripting.</span></span> <span data-ttu-id="a0b25-115">Para obter mais informações, consulte [atribuir licenças aos utilizadores](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) e [atribuir licenças às contas dos utilizadores com o Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span><span class="sxs-lookup"><span data-stu-id="a0b25-115">For more info, see [Assign licenses to users](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) and [Assign licenses to user accounts with Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span></span> 

<span data-ttu-id="a0b25-116">O Microsoft Support não presta assistência na criação de scripts, mas a documentação sobre a atribuição da licença Yammer está disponível.</span><span class="sxs-lookup"><span data-stu-id="a0b25-116">Microsoft Support does not provide assistance with creating scripts, but documentation on Yammer license assignment is available.</span></span> <span data-ttu-id="a0b25-117">Para obter mais informações, consulte [as licenças Manage Yammer utilizando o Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span><span class="sxs-lookup"><span data-stu-id="a0b25-117">For more info, see [Manage Yammer licenses by using Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span></span>