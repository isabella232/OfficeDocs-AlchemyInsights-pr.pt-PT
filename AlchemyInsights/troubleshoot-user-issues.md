---
title: Problemas de problemas com os utilizadores
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7813"
- "9004358"
ms.openlocfilehash: d9964e50bdea0c41ac14ab3783b579034b5f2c8c
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901334"
---
# <a name="announcements"></a><span data-ttu-id="95e45-102">Anúncios</span><span class="sxs-lookup"><span data-stu-id="95e45-102">Announcements</span></span>

<span data-ttu-id="95e45-103">Siga as orientações da Google sobre a compatibilidade dos testes para testar se as suas apps estão afetadas.</span><span class="sxs-lookup"><span data-stu-id="95e45-103">Follow Google's guidance on testing compatibility to test whether your apps are affected.</span></span> <span data-ttu-id="95e45-104">A orientação da Google está disponível em https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support .</span><span class="sxs-lookup"><span data-stu-id="95e45-104">Google's guidance is available in https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support.</span></span>

<span data-ttu-id="95e45-105">Certifique-se de que utiliza o webview do sistema ou o navegador do sistema ao assinar nos seus utilizadores com contas google de consumo.</span><span class="sxs-lookup"><span data-stu-id="95e45-105">Ensure you use the system webview or system browser when signing in your users with consumer Google accounts.</span></span> <span data-ttu-id="95e45-106">Para obter mais informações, consulte [Problemas de sessão de sessão para aplicações usando apenas o navegador Chrome](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).</span><span class="sxs-lookup"><span data-stu-id="95e45-106">For more information, see [Issues signing in to application(s) using Chrome browser only](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).</span></span>


<span data-ttu-id="95e45-107">**Não posso criar um novo utilizador no meu diretório AD Azure**</span><span class="sxs-lookup"><span data-stu-id="95e45-107">**I can't create a new user in my Azure AD directory**</span></span>

<span data-ttu-id="95e45-108">Para resolver problemas com a questão de não ser capaz de criar um novo utilizador em Azure AD, execute os seguintes passos:</span><span class="sxs-lookup"><span data-stu-id="95e45-108">To troubleshoot the issue of not being able to create a new user in Azure AD, perform the following steps:</span></span>

1. <span data-ttu-id="95e45-109">Certifique-se de que está autorizado a criar um novo utilizador padrão.</span><span class="sxs-lookup"><span data-stu-id="95e45-109">Ensure that you are authorized to create a new standard user.</span></span> <span data-ttu-id="95e45-110">Apenas o papel de administrador global ou administrador de utilizador no Azure Ative Directory (AD) pode criar um novo utilizador padrão.</span><span class="sxs-lookup"><span data-stu-id="95e45-110">Only the global administrator or user administrator role in Azure Active Directory (AD) can create a new standard user.</span></span> <span data-ttu-id="95e45-111">Se não estiver numa destas funções, peça a um administrador que o adicione a uma destas funções ou que crie a nova conta de utilizador para si.</span><span class="sxs-lookup"><span data-stu-id="95e45-111">If you're not in one of these roles, ask an administrator to add you to one of these roles or to create the new user account for you.</span></span>
2. <span data-ttu-id="95e45-112">Certifique-se de que o nome de utilizador está num domínio verificado no seu AD Azure.</span><span class="sxs-lookup"><span data-stu-id="95e45-112">Ensure that the user name is in a domain that is verified in your Azure AD.</span></span> <span data-ttu-id="95e45-113">Se não tiver nenhum nome de domínio personalizado verificado no seu AD Azure, pode utilizar o seu domínio inicial AD Azure, que termina com \*.onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="95e45-113">If you do not have any verified custom domain names in your Azure AD, you can use your Azure AD initial domain, which ends with \*.onmicrosoft.com.</span></span>
3. <span data-ttu-id="95e45-114">Certifique-se de que o nome de utilizador está num domínio que não é federado para Azure AD a partir do seu AD no local.</span><span class="sxs-lookup"><span data-stu-id="95e45-114">Ensure that the user name is in a domain that is not federated to Azure AD from your on-premises AD.</span></span> <span data-ttu-id="95e45-115">Os utilizadores não podem ser adicionados na nuvem com nomes de domínio que são federados do local.</span><span class="sxs-lookup"><span data-stu-id="95e45-115">Users cannot be added in the cloud with domain names that are federated from on-premises.</span></span>
4. <span data-ttu-id="95e45-116">Certifique-se de que nenhum outro utilizador ou contacto já tem o nome de utilizador que pretende atribuir ao novo utilizador.</span><span class="sxs-lookup"><span data-stu-id="95e45-116">Ensure that no other user or contact already has the user name that you want to assign to the new user.</span></span> <span data-ttu-id="95e45-117">Os nomes de utilizador devem ser únicos em todo o Azure AD.</span><span class="sxs-lookup"><span data-stu-id="95e45-117">User names must be unique across Azure AD.</span></span>
5. <span data-ttu-id="95e45-118">Consulte [as funções e administradores da AD Azure](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) para o seu AZure AD.</span><span class="sxs-lookup"><span data-stu-id="95e45-118">See [Azure AD roles and administrators](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) for your Azure AD.</span></span>
6. <span data-ttu-id="95e45-119">Consulte os [nomes de domínio](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Domains) do seu AD Azure.</span><span class="sxs-lookup"><span data-stu-id="95e45-119">See the [domain names](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Domains) for your Azure AD.</span></span>
7. <span data-ttu-id="95e45-120">[Reveja os registos de auditoria](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Audit) para ver informações mais detalhadas sobre um utilizador recentemente criado ou eliminado, como quem realizou a ação e quando.</span><span class="sxs-lookup"><span data-stu-id="95e45-120">Review [Audit logs](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Audit) to see more detailed information about a recently created or deleted user like who performed the action and when.</span></span>
8. <span data-ttu-id="95e45-121">Para obter mais informações sobre a adição de novos utilizadores, consulte [utilizar o portal Azure para criar um novo utilizador no seu AD Azure.](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)</span><span class="sxs-lookup"><span data-stu-id="95e45-121">For more information on adding new users, see [Use the Azure portal to create a new user in your Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory) .</span></span>
9. <span data-ttu-id="95e45-122">Para obter mais informações sobre permissões de função de administrador em Azure AD, consulte [as funções administrativas da AZure AD](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95e45-122">For more information on administrator role permissions in Azure AD, see [Azure AD administrative roles](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference).</span></span>
10. <span data-ttu-id="95e45-123">Para obter mais informações sobre a criação de um utilizador que utilize a Azure AD Powershell, consulte [a Azure AD PowerShell para criar um novo utilizador](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser).</span><span class="sxs-lookup"><span data-stu-id="95e45-123">For details on creating a user using Azure AD Powershell, see [Azure AD PowerShell to create a new user](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser).</span></span>

<span data-ttu-id="95e45-124">**Problema com a inscrição de self-service**</span><span class="sxs-lookup"><span data-stu-id="95e45-124">**Problem with self-service sign up**</span></span>

<span data-ttu-id="95e45-125">Para resolver problemas no que diz respeito à inscrição de self-service, execute os seguintes passos:</span><span class="sxs-lookup"><span data-stu-id="95e45-125">To troubleshoot issues regarding self-service sign up, perform the following steps:</span></span>

1. <span data-ttu-id="95e45-126">Para utilizar a inscrição de self-service com as suas aplicações, primeiro ative a inscrição de self-service para o seu inquilino.</span><span class="sxs-lookup"><span data-stu-id="95e45-126">To use self-service sign-up with your applications, first enable self-service sign-up for your tenant.</span></span> 
2. <span data-ttu-id="95e45-127">Para ativar uma aplicação para suportar a inscrição de self-service, adicione-a ao fluxo do seu utilizador .</span><span class="sxs-lookup"><span data-stu-id="95e45-127">To enable an application to support self-service sign up, add it to your user flow .</span></span> <span data-ttu-id="95e45-128">Da próxima vez que for à página de login para essa aplicação, verá uma opção \**_Sem conta? Criar um!_* _.</span><span class="sxs-lookup"><span data-stu-id="95e45-128">The next time you go to the login page for that application, you'll see an option \**_No account? Create one!_* _.</span></span> <span data-ttu-id="95e45-129">Isto inicia o processo de inscrição de autosserviço.</span><span class="sxs-lookup"><span data-stu-id="95e45-129">This starts the self-service sign-up process.</span></span>
3. <span data-ttu-id="95e45-130">Para obter informações sobre como usar o self-service inscreva-se para preencher uma organização em Azure AD, consulte [o Self-service inscreva-se para Azure AD](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-self-service-signup).</span><span class="sxs-lookup"><span data-stu-id="95e45-130">For information on how to use self-service sign up to populate an organization in Azure AD, see [Self-service sign up for Azure AD](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-self-service-signup).</span></span>
4. <span data-ttu-id="95e45-131">Uma vez associado o fluxo do utilizador a uma ou mais aplicações, os utilizadores que visitarem essa aplicação poderão inscrever-se e obter uma conta de hóspedes utilizando as opções configuradas no fluxo do utilizador.</span><span class="sxs-lookup"><span data-stu-id="95e45-131">Once you associate the user flow with one or more applications, users who visit that app will be able to sign up and gain a guest account using the options configured in the user flow.</span></span> <span data-ttu-id="95e45-132">Para obter mais informações sobre a inscrição e a obtenção de uma conta de hóspedes, os utilizadores podem ver [a inscrição de Self-service para utilizadores convidados.](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-user-flow)</span><span class="sxs-lookup"><span data-stu-id="95e45-132">For more information on signing up and gaining a guest account, the users can see [Self-service sign-up for guest users](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-user-flow).</span></span>

<span data-ttu-id="95e45-133">_ *Problema de convidar um utilizador externo*\*</span><span class="sxs-lookup"><span data-stu-id="95e45-133">_ *Problem inviting an external user*\*</span></span>

<span data-ttu-id="95e45-134">Para resolver problemas em relação à convidar um utilizador externo, execute o seguinte passo:</span><span class="sxs-lookup"><span data-stu-id="95e45-134">To troubleshoot issues regarding inviting an external user, perform the following step:</span></span>

<span data-ttu-id="95e45-135">Certifique-se de que envia o convite de um utilizador para o endereço de e-mail que corresponde ao nome com o qual o utilizador assina.</span><span class="sxs-lookup"><span data-stu-id="95e45-135">Ensure that you send a user's invitation to the email address that matches the name that the user signs in with.</span></span> <span data-ttu-id="95e45-136">Se enviar o convite para o endereço de e-mail de procuração de um utilizador, o utilizador não pode resgatá-lo.</span><span class="sxs-lookup"><span data-stu-id="95e45-136">If you send the invitation to a user's proxy email address, the user can't redeem it.</span></span> <span data-ttu-id="95e45-137">Para mais informações, consulte [a documentação do Azure AD B2B](https://docs.microsoft.com/azure/active-directory/external-identities/).</span><span class="sxs-lookup"><span data-stu-id="95e45-137">For more information, see [Azure AD B2B documentation](https://docs.microsoft.com/azure/active-directory/external-identities/).</span></span>

<span data-ttu-id="95e45-138">**Não posso atribuir licenças a um utilizador.**</span><span class="sxs-lookup"><span data-stu-id="95e45-138">**I can't assign licenses to a user**</span></span>

<span data-ttu-id="95e45-139">Para resolver problemas relativos à atribuição de licenças a um utilizador, execute os seguintes passos:</span><span class="sxs-lookup"><span data-stu-id="95e45-139">To troubleshoot issues regarding assigning licenses to a user, perform the following steps:</span></span>

1. <span data-ttu-id="95e45-140">Para gerir as licenças de utilizador, certifique-se de que utiliza uma conta com uma das funções de administrador necessárias: administrador global, administrador de licença ou administrador do utilizador.</span><span class="sxs-lookup"><span data-stu-id="95e45-140">To manage user licenses, ensure that you use an account with one of the required administrator roles: global administrator, license administrator, or user administrator.</span></span> <span data-ttu-id="95e45-141">Pode verificar a função do utilizador no **separador função** do Diretório na lâmina do utilizador.</span><span class="sxs-lookup"><span data-stu-id="95e45-141">You can check the user’s role in the **Directory role** tab on the user blade.</span></span>
2. <span data-ttu-id="95e45-142">Se estiver a utilizar o portal Azure e a atribuição da licença estiver a falhar, clique na notificação no canto superior direito.</span><span class="sxs-lookup"><span data-stu-id="95e45-142">If you are using the Azure portal and license assignment is failing, click the notification in the upper-right corner.</span></span> <span data-ttu-id="95e45-143">Isto abre uma lâmina com detalhes sobre o que correu mal.</span><span class="sxs-lookup"><span data-stu-id="95e45-143">This opens a blade with details about what went wrong.</span></span> <span data-ttu-id="95e45-144">Na maioria dos casos, isso é suficiente para compreender e resolver o problema.</span><span class="sxs-lookup"><span data-stu-id="95e45-144">In most cases that is enough to understand and resolve the problem.</span></span>
3. <span data-ttu-id="95e45-145">Antes de uma licença poder ser atribuída a um utilizador, certifique-se de que a propriedade **De Localização de Utilização** está definida para o utilizador.</span><span class="sxs-lookup"><span data-stu-id="95e45-145">Before a license can be assigned to a user, ensure that the **Usage Location** property is set for the user.</span></span> <span data-ttu-id="95e45-146">Verifique se o utilizador tem a propriedade definida visualizando o **separador Perfil** na lâmina do utilizador.</span><span class="sxs-lookup"><span data-stu-id="95e45-146">Verify the user has that property set by viewing the **Profile** tab on the user blade.</span></span>
4. <span data-ttu-id="95e45-147">Certifique-se de que existem licenças disponíveis suficientes para o produto que está a tentar atribuir.</span><span class="sxs-lookup"><span data-stu-id="95e45-147">Ensure there are enough available licenses for the product you are trying to assign.</span></span> <span data-ttu-id="95e45-148">Pode ver o número de licenças disponíveis no portal Azure, no [Azure Ative Directory -> Licenses -> Todos os produtos](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/LicensesMenuBlade/Products).</span><span class="sxs-lookup"><span data-stu-id="95e45-148">You can see the number of available licenses in the Azure portal, at [Azure Active Directory -> Licenses -> All products](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/LicensesMenuBlade/Products).</span></span>
5. <span data-ttu-id="95e45-149">O utilizador pode já ter outra licença cujos serviços entram em conflito com os da nova licença que está a tentar atribuir.</span><span class="sxs-lookup"><span data-stu-id="95e45-149">The user may already have another license whose services conflict with those in the new license you are trying to assign.</span></span> <span data-ttu-id="95e45-150">Por exemplo, se o utilizador tiver o serviço Exchange Online (Plano 1) ativado, não poderá atribuir uma licença ao Exchange Online (Plano 2).</span><span class="sxs-lookup"><span data-stu-id="95e45-150">For example, if the user has the Exchange Online (Plan 1) service enabled, you won’t be able to assign a license with the Exchange Online (Plan 2).</span></span> <span data-ttu-id="95e45-151">Desative um dos serviços para permitir a nova atribuição de licença.</span><span class="sxs-lookup"><span data-stu-id="95e45-151">Disable one of the services to allow the new license assignment.</span></span> <span data-ttu-id="95e45-152">Se estiver a utilizar o portal Azure ou os cmdlets PowerShell, a página de detalhes do **problema** lista os serviços específicos que estão a causar o conflito.</span><span class="sxs-lookup"><span data-stu-id="95e45-152">If you are using the Azure portal or PowerShell cmdlets, the **problem details** page lists the specific services that are causing the conflict.</span></span>
6. <span data-ttu-id="95e45-153">Se estiver a tentar remover uma licença e isso estiver a falhar, o utilizador poderá ter outras licenças com serviços que dependem dos serviços que está a tentar remover.</span><span class="sxs-lookup"><span data-stu-id="95e45-153">If you are trying to remove a license and that is failing, the user might have other licenses with services that depend on the services you are trying to remove.</span></span> <span data-ttu-id="95e45-154">Se estiver a utilizar o portal Azure ou os cmdlets PowerShell, a mensagem de erro listará os serviços específicos que têm dependências.</span><span class="sxs-lookup"><span data-stu-id="95e45-154">If you are using the Azure portal or PowerShell cmdlets, the error message will list the specific services that have dependencies.</span></span>
7. <span data-ttu-id="95e45-155">Se quiser entender por que uma licença foi adicionada/removida de um utilizador (por exemplo, quem mais na sua organização pode ter feito alterações), verifique os registos de auditoria.</span><span class="sxs-lookup"><span data-stu-id="95e45-155">If you want to understand why a license was added/removed from a user (for example, who else in your organization may have made changes), check the audit logs.</span></span> <span data-ttu-id="95e45-156">Desatrei o filtro às **atividades de licença** para mostrar todas as modificações, incluindo o "ator" que as executou.</span><span class="sxs-lookup"><span data-stu-id="95e45-156">Set the filter to **license activities** to show all modifications, including the "actor" that performed them.</span></span>
8. <span data-ttu-id="95e45-157">Se estiver a utilizar o Exchange Online, alguns utilizadores do seu inquilino podem estar configurados incorretamente com o mesmo valor de endereço proxy.</span><span class="sxs-lookup"><span data-stu-id="95e45-157">If you are using Exchange Online, some users in your tenant may be incorrectly configured with the same proxy address value.</span></span> <span data-ttu-id="95e45-158">Nesses casos, pode ver mensagens de erro genéricas quando uma operação de licença falha.</span><span class="sxs-lookup"><span data-stu-id="95e45-158">In such cases, you may see generic error messages when a license operation fails.</span></span> <span data-ttu-id="95e45-159">[Este artigo](https://docs.microsoft.com/exchange/troubleshoot/administration/proxy-address-being-used) contém mais informações sobre este problema, incluindo informações sobre [como ligar-se ao Exchange Online utilizando o PowerShell remoto.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell) Para identificar quais utilizadores no seu inquilino, conter o mesmo endereço de procuração, execute este cmdlet Exchange Online:</span><span class="sxs-lookup"><span data-stu-id="95e45-159">[This article](https://docs.microsoft.com/exchange/troubleshoot/administration/proxy-address-being-used) contains more information about this problem, including information on [how to connect to Exchange Online using remote PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).To identify which users in your tenant, contain the same proxy address, execute this Exchange Online cmdlet:</span></span>

<span data-ttu-id="95e45-160">Correr</span><span class="sxs-lookup"><span data-stu-id="95e45-160">Run</span></span>

<span data-ttu-id="95e45-161">Get-Recipient | onde {$_. EmailAddresses -match <user principal name> } | nome fL, RecipientType,emailaddresses</span><span class="sxs-lookup"><span data-stu-id="95e45-161">Get-Recipient | where {$_.EmailAddresses -match <user principal name>} | fL Name, RecipientType,emailaddresses</span></span>




