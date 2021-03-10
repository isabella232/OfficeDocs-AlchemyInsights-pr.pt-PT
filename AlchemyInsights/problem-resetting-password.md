---
title: Palavra-passe de reposição de problemas
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: aa1eba1efef6a4c28aa6b9229071304093395922
ms.sourcegitcommit: 9a00005546c2fe473e3cea2b06e38c27eada88c4
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/09/2021
ms.locfileid: "50696274"
---
# <a name="problems-resetting-password"></a><span data-ttu-id="b9a51-102">Problemas na redefinição da palavra-passe</span><span class="sxs-lookup"><span data-stu-id="b9a51-102">Problems resetting password</span></span>

<span data-ttu-id="b9a51-103">Seguem-se alguns dos problemas que poderá enfrentar ao redefinir a palavra-passe e as possíveis soluções:</span><span class="sxs-lookup"><span data-stu-id="b9a51-103">Following are some of the issues that you might face when resetting password and the possible solutions:</span></span>

<span data-ttu-id="b9a51-104">**Estou tendo um problema com a palavra-passe não abrangida nas outras categorias**</span><span class="sxs-lookup"><span data-stu-id="b9a51-104">**I'm having an issue with password reset not covered in the other categories**</span></span>

- <span data-ttu-id="b9a51-105">Certifique-se de que está autorizado a redefinir palavras-passe.</span><span class="sxs-lookup"><span data-stu-id="b9a51-105">Ensure you are authorized to reset passwords.</span></span> <span data-ttu-id="b9a51-106">Apenas administradores globais, de palavra-passe e de utilizadores podem redefinir as palavras-passe do utilizador.</span><span class="sxs-lookup"><span data-stu-id="b9a51-106">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="b9a51-107">Os administradores globais também podem redefinir as palavras-passe de outros administradores privilegiados.</span><span class="sxs-lookup"><span data-stu-id="b9a51-107">Global administrators can also reset other privileged administrator's passwords.</span></span>
- <span data-ttu-id="b9a51-108">Certifique-se de que compreende os requisitos de licenciamento:</span><span class="sxs-lookup"><span data-stu-id="b9a51-108">Ensure that you understand the licensing requirements:</span></span>
    - <span data-ttu-id="b9a51-109">Deve ter pelo menos uma licença atribuída na sua organização</span><span class="sxs-lookup"><span data-stu-id="b9a51-109">You must have at least one license assigned in your organization</span></span>
        - <span data-ttu-id="b9a51-110">Utilizadores da Cloud - Qualquer Office 365 (O365) pagou SKU, ou Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="b9a51-110">Cloud only users - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
        - <span data-ttu-id="b9a51-111">Utilizadores em nuvem e/ou no local - Azure AD Premium P1 ou P2, Mobilidade Empresarial + Segurança (EMS) ou Empresa Produtiva Segura (SPE)</span><span class="sxs-lookup"><span data-stu-id="b9a51-111">Cloud and/or on-premises users - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
        - <span data-ttu-id="b9a51-112">Para ler mais sobre os requisitos de licenciamento consulte o artigo [Requisitos de licenciamento para a palavra-passe de autosserviço AZure AD repostos](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="b9a51-112">To read more about licensing requirements see the article [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="b9a51-113">**Estou com problemas em testar a política de reset da palavra-passe que estabeleci**</span><span class="sxs-lookup"><span data-stu-id="b9a51-113">**I'm having problems testing the password reset policy I set**</span></span>

- <span data-ttu-id="b9a51-114">As políticas recentemente aplicadas podem demorar vários minutos a replicar-se em todos os centros de dados e pontos finais.</span><span class="sxs-lookup"><span data-stu-id="b9a51-114">Recently applied policies can take several minutes to replicate across all data centers and end-points.</span></span> <span data-ttu-id="b9a51-115">A distância física do centro de dados também afetará a rapidez com que as mudanças são aplicadas.</span><span class="sxs-lookup"><span data-stu-id="b9a51-115">Physical distance from the data center will also affect how quickly changes are applied.</span></span>
- <span data-ttu-id="b9a51-116">Teste com um utilizador final, não um administrador, e piloto com um pequeno conjunto de utilizadores.</span><span class="sxs-lookup"><span data-stu-id="b9a51-116">Test with an end user, not an administrator, and pilot with a small set of users.</span></span> <span data-ttu-id="b9a51-117">As políticas configuradas no portal Azure aplicam-se apenas aos utilizadores finais e não aos administradores.</span><span class="sxs-lookup"><span data-stu-id="b9a51-117">The policies configured in the Azure portal ONLY apply to end-users, not administrators.</span></span> <span data-ttu-id="b9a51-118">A Microsoft aplica uma forte política de reset de senha de dois prazos para qualquer função de administrador do Azure (Exemplo: Administrador Global, Administrador de Ajuda, Administrador de Password, etc.)</span><span class="sxs-lookup"><span data-stu-id="b9a51-118">Microsoft enforces a strong default two-gate password reset policy for any Azure administrator role (Example: Global Administrator, Helpdesk Administrator, Password Administrator, etc.)</span></span>
    - <span data-ttu-id="b9a51-119">Saiba mais sobre [políticas para administradores.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)</span><span class="sxs-lookup"><span data-stu-id="b9a51-119">Learn more about [policies for administrators](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).</span></span>

<span data-ttu-id="b9a51-120">**Quero implementar o reset da palavra-passe, mas não quero que os meus utilizadores registem informações adicionais de segurança.**</span><span class="sxs-lookup"><span data-stu-id="b9a51-120">**I want to deploy password reset but I don't want to make my users register additional security info**</span></span>

<span data-ttu-id="b9a51-121">Preencha os dados para os seus utilizadores para que não tenham de o fazer!</span><span class="sxs-lookup"><span data-stu-id="b9a51-121">Pre-populate data for your users so they don't have to!</span></span> <span data-ttu-id="b9a51-122">- Como administrador, pode definir propriedades de telefone e e-mail para os seus utilizadores antes de lançar a palavra-passe para a sua organização.</span><span class="sxs-lookup"><span data-stu-id="b9a51-122">- As an administrator you can set phone and email properties for your users before rolling out password reset to your organization.</span></span> <span data-ttu-id="b9a51-123">Pode fazê-lo utilizando uma Ligação API, PowerShell ou AZure AD.</span><span class="sxs-lookup"><span data-stu-id="b9a51-123">You can do this using an API, PowerShell, or Azure AD Connect.</span></span> <span data-ttu-id="b9a51-124">Mais informações aqui:</span><span class="sxs-lookup"><span data-stu-id="b9a51-124">More information here:</span></span>
- [<span data-ttu-id="b9a51-125">Implementar a palavra-passe reiniciada sem exigir que os utilizadores se registem</span><span class="sxs-lookup"><span data-stu-id="b9a51-125">Deploying password reset without requiring users to register</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [<span data-ttu-id="b9a51-126">Que dados são usados por reset de senha</span><span class="sxs-lookup"><span data-stu-id="b9a51-126">What data is used by password reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="b9a51-127">**O botão de reset da palavra-passe está acinzentado**</span><span class="sxs-lookup"><span data-stu-id="b9a51-127">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="b9a51-128">Não está autorizado a redefinir as palavras-passe deste utilizador.</span><span class="sxs-lookup"><span data-stu-id="b9a51-128">You are not authorized to reset this user's passwords.</span></span> <span data-ttu-id="b9a51-129">Apenas administradores globais, de palavra-passe e de utilizadores podem redefinir as palavras-passe do utilizador.</span><span class="sxs-lookup"><span data-stu-id="b9a51-129">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="b9a51-130">Os administradores globais também podem redefinir as palavras-passe de outros administradores privilegiados.</span><span class="sxs-lookup"><span data-stu-id="b9a51-130">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="b9a51-131">**Não vejo a lâmina de reset da palavra-passe.**</span><span class="sxs-lookup"><span data-stu-id="b9a51-131">**I don't see the password reset blade**</span></span>

<span data-ttu-id="b9a51-132">Não está autorizado a redefinir palavras-passe.</span><span class="sxs-lookup"><span data-stu-id="b9a51-132">You are not authorized to reset passwords.</span></span> <span data-ttu-id="b9a51-133">Apenas administradores globais, de palavra-passe e de utilizadores podem redefinir as palavras-passe do utilizador.</span><span class="sxs-lookup"><span data-stu-id="b9a51-133">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="b9a51-134">Os administradores globais também podem redefinir as palavras-passe de outros administradores privilegiados.</span><span class="sxs-lookup"><span data-stu-id="b9a51-134">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="b9a51-135">**Não vejo a lâmina de integração no local no reset da palavra-passe**</span><span class="sxs-lookup"><span data-stu-id="b9a51-135">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="b9a51-136">A lâmina de integração no local só aparece em ambientes híbridos - o que significa que está a usar a gravação de passwords para manipular as palavras-passe do utilizador no local.</span><span class="sxs-lookup"><span data-stu-id="b9a51-136">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>
- <span data-ttu-id="b9a51-137">Não se vê esta lâmina se:</span><span class="sxs-lookup"><span data-stu-id="b9a51-137">You do not see this blade if:</span></span>
    - <span data-ttu-id="b9a51-138">Não está a usar o writeback da palavra-passe</span><span class="sxs-lookup"><span data-stu-id="b9a51-138">You are not using password writeback</span></span>
    - <span data-ttu-id="b9a51-139">Há um problema com a sua instalação/conectividade de writeback de palavra-passe</span><span class="sxs-lookup"><span data-stu-id="b9a51-139">There is a problem with your installation/connectivity of password writeback</span></span>
    - <span data-ttu-id="b9a51-140">Há um problema com a sua instalação/conectividade do Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="b9a51-140">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
    - <span data-ttu-id="b9a51-141">Para obter mais etapas de resolução de problemas para problemas com a gravação de password, consulte a secção [Descreva a palavra-passe de resolução de problemas](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="b9a51-141">For more troubleshooting steps for issues with password writeback, see the section [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="b9a51-142">**Não sei como redefinir a senha de um utilizador.**</span><span class="sxs-lookup"><span data-stu-id="b9a51-142">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="b9a51-143">Inscreva-se no portal Azure como um administrador apropriado.</span><span class="sxs-lookup"><span data-stu-id="b9a51-143">Sign in to the Azure portal as an appropriate admin.</span></span>
1. <span data-ttu-id="b9a51-144">Aceda à lâmina dos Utilizadores e grupos, selecione **Todos os Utilizadores**.</span><span class="sxs-lookup"><span data-stu-id="b9a51-144">Go to the Users and groups blade, select **All Users**.</span></span>
1. <span data-ttu-id="b9a51-145">Selecione um utilizador da lista.</span><span class="sxs-lookup"><span data-stu-id="b9a51-145">Select a user from the list.</span></span>
1. <span data-ttu-id="b9a51-146">Para o utilizador selecionado, selecione **'Visão geral'** e, em seguida, na barra de comando, clique em **Redefinir a palavra-passe**.</span><span class="sxs-lookup"><span data-stu-id="b9a51-146">For the selected user, select **Overview**, and then in the command bar, click **Reset password**.</span></span>
1. <span data-ttu-id="b9a51-147">Siga as instruções no ecrã.</span><span class="sxs-lookup"><span data-stu-id="b9a51-147">Follow the instructions on the screen.</span></span>
    - <span data-ttu-id="b9a51-148">Apenas resets realizados através da gravação de senha de suporte do portal Azure.</span><span class="sxs-lookup"><span data-stu-id="b9a51-148">Only resets performed through the Azure portal support password writeback.</span></span>

<span data-ttu-id="b9a51-149">**Repus a palavra-passe de um utilizador no local a partir do portal de administração do Office 365 ou da aplicação móvel do Office 365, mas o utilizador ainda não consegue iniciar sposição.**</span><span class="sxs-lookup"><span data-stu-id="b9a51-149">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="b9a51-150">A writeback de palavra-passe não é suportada neste portal.</span><span class="sxs-lookup"><span data-stu-id="b9a51-150">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="b9a51-151">Repor novamente a palavra-passe do utilizador no portal Azure - portal.azure.com</span><span class="sxs-lookup"><span data-stu-id="b9a51-151">Reset the user's password again in the Azure portal - portal.azure.com</span></span>

