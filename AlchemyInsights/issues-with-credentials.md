---
title: Problemas com credenciais
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
- "9004330"
- "7723"
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063684"
---
# <a name="issues-with-credentials"></a><span data-ttu-id="2cdf8-102">Problemas com credenciais</span><span class="sxs-lookup"><span data-stu-id="2cdf8-102">Issues with credentials</span></span>

<span data-ttu-id="2cdf8-103">[A plataforma de identidade da Microsoft e o fluxo de credenciais de cliente OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) descrevem como programar diretamente contra o fluxo de concessão de credenciais de cliente OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="2cdf8-103">[Microsoft identity platform and the OAuth 2.0 client credentials flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) describes how to program directly against the OAuth 2.0 client credentials grant flow.</span></span>

<span data-ttu-id="2cdf8-104">**Como posso gerir as credenciais de senha ou certificado de uma aplicação?**</span><span class="sxs-lookup"><span data-stu-id="2cdf8-104">**How do I manage an application's password or certificate credentials?**</span></span>

<span data-ttu-id="2cdf8-105">No CLI Azure, pode utilizar [a credencial de aplicação ad az](https://docs.microsoft.com/cli/azure/ad/app/credential) para eliminar, listar ou redefinir as credenciais de senha ou certificado de uma aplicação.</span><span class="sxs-lookup"><span data-stu-id="2cdf8-105">In the Azure CLI, you can use [az ad app credential](https://docs.microsoft.com/cli/azure/ad/app/credential) to delete, list, or reset an application's password or certificate credentials.</span></span>

<span data-ttu-id="2cdf8-106">**Como é que os meus utilizadores repõei as suas palavras-passe?**</span><span class="sxs-lookup"><span data-stu-id="2cdf8-106">**How do my users reset their passwords?**</span></span>

<span data-ttu-id="2cdf8-107">Os utilizadores precisam de [se registar para redefinição da palavra-passe de autosserviço](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) antes de poderem redefinir as suas palavras-passe.</span><span class="sxs-lookup"><span data-stu-id="2cdf8-107">Users need to [register for self-service password reset](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) before they can reset their passwords.</span></span> <span data-ttu-id="2cdf8-108">Uma vez registado um utilizador, podem seguir as instruções deste artigo para redefinir a sua palavra-passe: [Redefinir o seu trabalho ou a palavra-passe da escola](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).</span><span class="sxs-lookup"><span data-stu-id="2cdf8-108">Once a user has registered, they can follow the instructions in this article to reset their password: [Reset your work or school password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).</span></span>

<span data-ttu-id="2cdf8-109">**Como é que os meus utilizadores mudam as suas palavras-passe?**</span><span class="sxs-lookup"><span data-stu-id="2cdf8-109">**How do my users change their passwords?**</span></span>

<span data-ttu-id="2cdf8-110">Os utilizadores podem seguir os passos deste artigo para alterar as suas palavras-passe: [Como alterar a sua palavra-passe](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).</span><span class="sxs-lookup"><span data-stu-id="2cdf8-110">Users can follow the steps in this article to change their passwords: [How to change your password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).</span></span>
<span data-ttu-id="2cdf8-111">Também podem [Gerir palavras-passe de aplicações para verificação em duas etapas.](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)</span><span class="sxs-lookup"><span data-stu-id="2cdf8-111">They can also [Manage app passwords for two-step verification](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).</span></span>

<span data-ttu-id="2cdf8-112">**O meu utilizador está a ter um erro ao alterar ou redefinir a sua palavra-passe**</span><span class="sxs-lookup"><span data-stu-id="2cdf8-112">**My user is getting an error when changing or resetting their password**</span></span>

<span data-ttu-id="2cdf8-113">Este link fornecerá informações sobre problemas comuns que podem surgir quando um utilizador está a tentar redefinir a sua palavra-passe: [Problemas comuns e suas soluções](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span><span class="sxs-lookup"><span data-stu-id="2cdf8-113">This link will provide information on common problems that can arise when a user is trying to reset their password: [Common problems and their solutions](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span></span>

<span data-ttu-id="2cdf8-114">**Estou a ter problemas em redefinir a senha de um utilizador.**</span><span class="sxs-lookup"><span data-stu-id="2cdf8-114">**I'm having a problem resetting a user's password**</span></span>

- <span data-ttu-id="2cdf8-115">Certifique-se de que está autorizado a redefinir palavras-passe.</span><span class="sxs-lookup"><span data-stu-id="2cdf8-115">Make sure you are authorized to reset passwords.</span></span> <span data-ttu-id="2cdf8-116">*Apenas administradores globais, de palavra-passe e de utilizadores podem redefinir as palavras-passe do utilizador.*</span><span class="sxs-lookup"><span data-stu-id="2cdf8-116">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="2cdf8-117">Os administradores globais também podem redefinir as palavras-passe de outros administradores privilegiados.</span><span class="sxs-lookup"><span data-stu-id="2cdf8-117">Global administrators can also reset other privileged administrator's passwords.</span></span>

- <span data-ttu-id="2cdf8-118">Certifique-se de compreender os requisitos de licenciamento:</span><span class="sxs-lookup"><span data-stu-id="2cdf8-118">Make sure you understand the licensing requirements:</span></span>

  - <span data-ttu-id="2cdf8-119">Deve ter pelo menos uma licença atribuída na sua organização:</span><span class="sxs-lookup"><span data-stu-id="2cdf8-119">You must have at least one license assigned in your organization:</span></span>
    - <span data-ttu-id="2cdf8-120">**Utilizadores da Cloud -** Qualquer Office 365 (O365) pagou SKU, ou Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="2cdf8-120">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
    - <span data-ttu-id="2cdf8-121">**Utilizadores em nuvem e/ou no local** - Azure AD Premium P1 ou P2, Mobilidade Empresarial + Segurança (EMS) ou Empresa Produtiva Segura (SPE)</span><span class="sxs-lookup"><span data-stu-id="2cdf8-121">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="2cdf8-122">Para saber mais sobre os requisitos de licenciamento, consulte [os requisitos de licenciamento para a Azure AD autosserviço de autosserviço reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).</span><span class="sxs-lookup"><span data-stu-id="2cdf8-122">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).</span></span>
- <span data-ttu-id="2cdf8-123">Para redefinir a palavra-passe de um utilizador, encontre o utilizador no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="2cdf8-123">To reset a user's password, find the user in Azure AD.</span></span> <span data-ttu-id="2cdf8-124">Em seguida, na lâmina de visão geral para esse utilizador, clique no botão "redefinir a palavra-passe".</span><span class="sxs-lookup"><span data-stu-id="2cdf8-124">Then, on the overview blade for that user, click the "reset password" button.</span></span>

<span data-ttu-id="2cdf8-125">**O botão de reset da palavra-passe está acinzentado**</span><span class="sxs-lookup"><span data-stu-id="2cdf8-125">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="2cdf8-126">Não está autorizado a redefinir as palavras-passe **deste** utilizador.</span><span class="sxs-lookup"><span data-stu-id="2cdf8-126">You are not authorized to reset **this** user's passwords.</span></span> <span data-ttu-id="2cdf8-127">*Apenas administradores globais, de palavra-passe e de utilizadores podem redefinir as palavras-passe do utilizador.*</span><span class="sxs-lookup"><span data-stu-id="2cdf8-127">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="2cdf8-128">Os administradores globais também podem redefinir as palavras-passe de outros administradores privilegiados.</span><span class="sxs-lookup"><span data-stu-id="2cdf8-128">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="2cdf8-129">**Não vejo a lâmina de reset da palavra-passe.**</span><span class="sxs-lookup"><span data-stu-id="2cdf8-129">**I don't see the password reset blade**</span></span>

<span data-ttu-id="2cdf8-130">Não está autorizado a redefinir palavras-passe.</span><span class="sxs-lookup"><span data-stu-id="2cdf8-130">You are not authorized to reset passwords.</span></span> <span data-ttu-id="2cdf8-131">*Apenas administradores globais, de palavra-passe e de utilizadores podem redefinir as palavras-passe do utilizador.*</span><span class="sxs-lookup"><span data-stu-id="2cdf8-131">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="2cdf8-132">Os administradores globais também podem redefinir as palavras-passe de outros administradores privilegiados.</span><span class="sxs-lookup"><span data-stu-id="2cdf8-132">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="2cdf8-133">**Não vejo a lâmina de integração no local no reset da palavra-passe**</span><span class="sxs-lookup"><span data-stu-id="2cdf8-133">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="2cdf8-134">A lâmina de integração no local só aparece em ambientes híbridos - o que significa que está a usar a gravação de passwords para manipular as palavras-passe do utilizador no local.</span><span class="sxs-lookup"><span data-stu-id="2cdf8-134">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>

- <span data-ttu-id="2cdf8-135">Não se vê esta lâmina se:</span><span class="sxs-lookup"><span data-stu-id="2cdf8-135">You do not see this blade if:</span></span>

  - <span data-ttu-id="2cdf8-136">Não está a usar o writeback da palavra-passe</span><span class="sxs-lookup"><span data-stu-id="2cdf8-136">You are not using password writeback</span></span>
  - <span data-ttu-id="2cdf8-137">Há um problema com a sua instalação/conectividade de writeback de palavra-passe</span><span class="sxs-lookup"><span data-stu-id="2cdf8-137">There is a problem with your installation/connectivity of password writeback</span></span>
  - <span data-ttu-id="2cdf8-138">Há um problema com a sua instalação/conectividade do Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="2cdf8-138">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
  - <span data-ttu-id="2cdf8-139">Para obter mais etapas de resolução de problemas para problemas com a writeback de password, consulte [o writeback da palavra-passe de Resolução de Problemas](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span><span class="sxs-lookup"><span data-stu-id="2cdf8-139">For more troubleshooting steps for issues with password writeback, see [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span></span>

<span data-ttu-id="2cdf8-140">**Não sei como redefinir a senha de um utilizador.**</span><span class="sxs-lookup"><span data-stu-id="2cdf8-140">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="2cdf8-141">Inscreva-se no portal Azure como um administrador apropriado.</span><span class="sxs-lookup"><span data-stu-id="2cdf8-141">Sign in to the Azure portal as an appropriate admin.</span></span>
2. <span data-ttu-id="2cdf8-142">Aceda à lâmina **dos Utilizadores e grupos,** selecione **Todos os Utilizadores**.</span><span class="sxs-lookup"><span data-stu-id="2cdf8-142">Go to the **Users and groups** blade, select **All Users**.</span></span>
3. <span data-ttu-id="2cdf8-143">Selecione um utilizador da lista.</span><span class="sxs-lookup"><span data-stu-id="2cdf8-143">Select a user from the list.</span></span>
4. <span data-ttu-id="2cdf8-144">Para o utilizador selecionado, selecione **'Visão geral'** e, em seguida, na barra de comando, **selecione Redefinir a palavra-passe**.</span><span class="sxs-lookup"><span data-stu-id="2cdf8-144">For the selected user, select **Overview**, and then in the command bar, select **Reset password**.</span></span>
5. <span data-ttu-id="2cdf8-145">Selecione o botão **de palavra-passe Reset** e siga as instruções no ecrã.</span><span class="sxs-lookup"><span data-stu-id="2cdf8-145">Select the **Reset password** button and follow the instructions on the screen.</span></span>
    - <span data-ttu-id="2cdf8-146">Apenas resets realizados através da gravação de senha de suporte do **portal Azure.**</span><span class="sxs-lookup"><span data-stu-id="2cdf8-146">Only resets performed through the **Azure portal** support password writeback.</span></span>

<span data-ttu-id="2cdf8-147">**Repus a palavra-passe de um utilizador no local a partir do portal de administração do Office 365 ou da aplicação móvel do Office 365, mas o utilizador ainda não consegue iniciar sposição.**</span><span class="sxs-lookup"><span data-stu-id="2cdf8-147">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="2cdf8-148">A writeback de palavra-passe não é suportada neste portal.</span><span class="sxs-lookup"><span data-stu-id="2cdf8-148">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="2cdf8-149">Repor novamente a palavra-passe do utilizador no portal Azure.</span><span class="sxs-lookup"><span data-stu-id="2cdf8-149">Reset the user's password again in the Azure portal.</span></span>
