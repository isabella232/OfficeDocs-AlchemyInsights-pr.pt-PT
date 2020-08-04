---
title: Problemas na utilização da consola de administração Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 7a36d502a92d360b06336ccfa6183f666f0260ab
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555389"
---
# <a name="problems-using-the-intune-admin-console"></a><span data-ttu-id="7e9df-102">Problemas na utilização da consola de administração Intune</span><span class="sxs-lookup"><span data-stu-id="7e9df-102">Problems using the Intune admin console</span></span>

<span data-ttu-id="7e9df-103">**"Acesso negado" ao navegar no portal de administração Intune.**</span><span class="sxs-lookup"><span data-stu-id="7e9df-103">**"Access denied" when navigating the Intune admin portal.**</span></span>

- <span data-ttu-id="7e9df-104">Se for membro de uma função personalizada Intune, certifique-se de que uma licença Intune ou Enterprise Mobility Suite (EMS) é atribuída à sua conta.</span><span class="sxs-lookup"><span data-stu-id="7e9df-104">If you are a member of an Intune custom role, ensure that an Intune or Enterprise Mobility Suite (EMS) license is assigned to your account.</span></span>
- <span data-ttu-id="7e9df-105">Se estiver a utilizar o Gestor de Configuração para gerir dispositivos, verifique se não faz parte da coleção de utilizadores Intune para o Gestor de Configuração MDM.</span><span class="sxs-lookup"><span data-stu-id="7e9df-105">If you are using Configuration Manager to manage devices, verify you are not part of the Intune user collection for Configuration Manager MDM.</span></span>
- <span data-ttu-id="7e9df-106">Verifique se lhe foi atribuídas as permissões adequadas de controlo de administração (RBAC) na lâmina de funções Intune.</span><span class="sxs-lookup"><span data-stu-id="7e9df-106">Verify that you have been assigned the appropriate role-based administration control (RBAC) permissions in the Intune roles blade.</span></span>
- <span data-ttu-id="7e9df-107">Verifique se o grupo utilizado não é uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="7e9df-107">Verify the group used is not a distribution list.</span></span> <span data-ttu-id="7e9df-108">Intune no portal Azure apenas suporta contas de utilizadores que pertencem a grupos de segurança do Azure Ative Directory.</span><span class="sxs-lookup"><span data-stu-id="7e9df-108">Intune in the Azure portal only supports user accounts that belong to Azure Active Directory security groups.</span></span> <span data-ttu-id="7e9df-109">Reveja os seus grupos no portal Azure > Grupos **Intune**  >  **Groups**, ou no portal Azure > **Azure Ative Directory**.</span><span class="sxs-lookup"><span data-stu-id="7e9df-109">Review your groups in the Azure portal > **Intune** > **Groups**, or in Azure portal > **Azure Active Directory**.</span></span>

<span data-ttu-id="7e9df-110">**O utilizador tem demasiadas permissões para o papel intune atribuído**</span><span class="sxs-lookup"><span data-stu-id="7e9df-110">**User has too many permissions for assigned Intune role**</span></span>

<span data-ttu-id="7e9df-111">Aconselhe o utilizador a ir às funções **Intune**  >  **Intune**  >  **As minhas permissões**  >  **Exportar** para rever permissões concedidas.</span><span class="sxs-lookup"><span data-stu-id="7e9df-111">Advise the user to go to **Intune** > **Intune roles** > **My permissions** > **Export** to review granted permissions.</span></span>

<span data-ttu-id="7e9df-112">**Adicionei um grupo de âmbito a um papel, mas os utilizadores nessa função ainda vêem outros utilizadores ou dispositivos.**</span><span class="sxs-lookup"><span data-stu-id="7e9df-112">**I added a scope group to a role, but users in that role still see other users or devices.**</span></span>

<span data-ttu-id="7e9df-113">Os grupos de âmbito não filtram os utilizadores ou dispositivos.</span><span class="sxs-lookup"><span data-stu-id="7e9df-113">Scope groups do not filter out users or devices.</span></span> <span data-ttu-id="7e9df-114">Grupos de âmbito:</span><span class="sxs-lookup"><span data-stu-id="7e9df-114">Scope groups:</span></span>

- <span data-ttu-id="7e9df-115">Limite a quem os utilizadores podem atribuir políticas ou aplicações.</span><span class="sxs-lookup"><span data-stu-id="7e9df-115">Limit who users can assign policies or applications to.</span></span>
- <span data-ttu-id="7e9df-116">Permitir que apenas utilizadores específicos executem tarefas remotas em dispositivos.</span><span class="sxs-lookup"><span data-stu-id="7e9df-116">Allow only specific users to run remote tasks on devices.</span></span>

<span data-ttu-id="7e9df-117">Para obter mais informações sobre grupos de âmbito, consulte [o controlo de acesso baseado em funções (RBAC) com o Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="7e9df-117">For more information about scope groups, see  [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="7e9df-118">**Adicionei um utilizador a um papel intune, mas eles ainda têm acesso total à consola de administração Intune.**</span><span class="sxs-lookup"><span data-stu-id="7e9df-118">**I added a user to an Intune role but they still have full access to the Intune admin console.**</span></span>

<span data-ttu-id="7e9df-119">Navegue para Intune > **Utilizadores** no portal Azure e verifique se o utilizador não está atribuído a nenhuma das seguintes funções no portal Azure:</span><span class="sxs-lookup"><span data-stu-id="7e9df-119">Navigate to Intune > **Users** in the Azure portal and verify that the user is not assigned to any of the following roles in the Azure portal:</span></span>

- <span data-ttu-id="7e9df-120">Administrador global</span><span class="sxs-lookup"><span data-stu-id="7e9df-120">Global administrator</span></span>
- <span data-ttu-id="7e9df-121">Administrador de serviço intune</span><span class="sxs-lookup"><span data-stu-id="7e9df-121">Intune service administrator</span></span>
- <span data-ttu-id="7e9df-122">Administrador do SharePoint</span><span class="sxs-lookup"><span data-stu-id="7e9df-122">SharePoint administrator</span></span>

<span data-ttu-id="7e9df-123">Para obter mais informações, consulte [o controlo de acesso baseado em funções (RBAC) com o Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="7e9df-123">For more info, see [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="7e9df-124">**Problemas de acesso**</span><span class="sxs-lookup"><span data-stu-id="7e9df-124">**Access Issues**</span></span>

<span data-ttu-id="7e9df-125">Para mais informações, veja [não pode assinar no Office 365, Azure ou Intune.](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune)</span><span class="sxs-lookup"><span data-stu-id="7e9df-125">For more info, see [You can't sign in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span></span>