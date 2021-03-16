---
title: Criar utilizador
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003231"
- "9403"
ms.openlocfilehash: 742ff857141d08031302fdcff7e49b3eef90e0f7
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747023"
---
# <a name="create-user"></a><span data-ttu-id="64ab8-102">Criar utilizador</span><span class="sxs-lookup"><span data-stu-id="64ab8-102">Create user</span></span>

<span data-ttu-id="64ab8-103">**ANÚNCIO:**</span><span class="sxs-lookup"><span data-stu-id="64ab8-103">**ANNOUNCEMENT:**</span></span>

- <span data-ttu-id="64ab8-104">[Depreciação do suporte de sing-in webView do Google a partir de 4 de janeiro de 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) .</span><span class="sxs-lookup"><span data-stu-id="64ab8-104">[Deprecation of WebView sign-in support from Google starting January 4, 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) .</span></span> <span data-ttu-id="64ab8-105">Teste se as suas apps podem ser afetadas seguindo a [orientação da Google](https://go.microsoft.com/fwlink/?linkid=2157323) sobre a compatibilidade dos testes.</span><span class="sxs-lookup"><span data-stu-id="64ab8-105">Test whether your apps may be affected by following [Google’s guidance](https://go.microsoft.com/fwlink/?linkid=2157323) on testing compatibility.</span></span>
- <span data-ttu-id="64ab8-106">Certifique-se de que utiliza o webview do sistema ou o navegador do sistema ao assinar nos seus utilizadores com contas google de consumo.</span><span class="sxs-lookup"><span data-stu-id="64ab8-106">Make sure you use the system webview or system browser when signing in your users with consumer Google accounts.</span></span> <span data-ttu-id="64ab8-107">Para obter mais informações, consulte [Problemas de sessão de sessão para aplicações usando apenas o navegador Chrome](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).</span><span class="sxs-lookup"><span data-stu-id="64ab8-107">For more information, see [Issues signing in to application(s) using Chrome browser only](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).</span></span>

<span data-ttu-id="64ab8-108">**Não posso criar um novo utilizador no meu diretório AD Azure**</span><span class="sxs-lookup"><span data-stu-id="64ab8-108">**I can't create a new user in my Azure AD directory**</span></span>

1. <span data-ttu-id="64ab8-109">Certifique-se de que está autorizado a criar um novo utilizador padrão.</span><span class="sxs-lookup"><span data-stu-id="64ab8-109">Ensure that you are authorized to create a new standard user.</span></span> <span data-ttu-id="64ab8-110">Apenas o administrador global ou o papel de administrador do utilizador no Azure Ative Directory (AD) podem criar um novo utilizador padrão.</span><span class="sxs-lookup"><span data-stu-id="64ab8-110">Only the Global administrator or User administrator role in Azure Active Directory (AD) can create a new standard user.</span></span> <span data-ttu-id="64ab8-111">Se não estiver numa destas funções, peça a um administrador que o adicione a uma destas funções ou que crie a nova conta de utilizador para si.</span><span class="sxs-lookup"><span data-stu-id="64ab8-111">If you're not in one of these roles, ask an administrator to add you to one of these roles or to create the new user account for you.</span></span>
1. <span data-ttu-id="64ab8-112">Certifique-se de que o nome de utilizador está num domínio verificado no seu AD Azure.</span><span class="sxs-lookup"><span data-stu-id="64ab8-112">Ensure that the user name is in a domain that is verified in your Azure AD.</span></span> <span data-ttu-id="64ab8-113">Se não tiver nenhum nome de domínio personalizado verificado no seu AD Azure, pode utilizar o seu domínio inicial AD Azure, que termina com \*.onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="64ab8-113">If you do not have any verified custom domain names in your Azure AD, you can use your Azure AD initial domain, which ends with \*.onmicrosoft.com.</span></span>
1. <span data-ttu-id="64ab8-114">Certifique-se de que o nome de utilizador está num domínio que não é federado para Azure AD a partir do seu AD no local.</span><span class="sxs-lookup"><span data-stu-id="64ab8-114">Ensure that the user name is in a domain that is not federated to Azure AD from your on-premises AD.</span></span> <span data-ttu-id="64ab8-115">Os utilizadores não podem ser adicionados na nuvem com nomes de domínio que são federados do local.</span><span class="sxs-lookup"><span data-stu-id="64ab8-115">Users cannot be added in the cloud with domain names that are federated from on-premises.</span></span>
1. <span data-ttu-id="64ab8-116">Certifique-se de que nenhum outro utilizador ou contacto já tem o nome de utilizador que pretende atribuir ao novo utilizador.</span><span class="sxs-lookup"><span data-stu-id="64ab8-116">Ensure that no other user or contact already has the user name that you want to assign to the new user.</span></span> <span data-ttu-id="64ab8-117">Os nomes de utilizador devem ser únicos em todo o Azure AD.</span><span class="sxs-lookup"><span data-stu-id="64ab8-117">User names must be unique across Azure AD.</span></span>
1. <span data-ttu-id="64ab8-118">Consulte [as funções e administradores da AD Azure](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) para o seu AZure AD.</span><span class="sxs-lookup"><span data-stu-id="64ab8-118">See [Azure AD roles and administrators](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) for your Azure AD.</span></span>
1. <span data-ttu-id="64ab8-119">Consulte os [nomes de domínio](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) do seu AD Azure.</span><span class="sxs-lookup"><span data-stu-id="64ab8-119">See the [domain names](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) for your Azure AD.</span></span>
1. <span data-ttu-id="64ab8-120">[Reveja os registos de auditoria](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) para ver informações mais detalhadas sobre um utilizador recentemente criado ou eliminado, como quem realizou a ação e quando.</span><span class="sxs-lookup"><span data-stu-id="64ab8-120">Review [Audit logs](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) to see more detailed information about a recently created or deleted user like who performed the action and when.</span></span>
1. <span data-ttu-id="64ab8-121">Para obter mais informações sobre a adição de novos utilizadores, consulte [utilizar o portal Azure para criar um novo utilizador no seu AD Azure.](/azure/active-directory/active-directory-users-create-azure-portal)</span><span class="sxs-lookup"><span data-stu-id="64ab8-121">For more information on adding new users, see [Use the Azure portal to create a new user in your Azure AD](/azure/active-directory/active-directory-users-create-azure-portal).</span></span>
1. <span data-ttu-id="64ab8-122">[Funções administrativas Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles): Permissões de função de administrador no Azure Ative Directory</span><span class="sxs-lookup"><span data-stu-id="64ab8-122">[Azure AD administrative roles](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles): Administrator role permissions in Azure Active Directory</span></span>
1. <span data-ttu-id="64ab8-123">Também pode [utilizar o Azure AD PowerShell para criar um novo utilizador](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser?view=azureadps-2.0).</span><span class="sxs-lookup"><span data-stu-id="64ab8-123">You can also [use Azure AD PowerShell to create a new user](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser?view=azureadps-2.0).</span></span>