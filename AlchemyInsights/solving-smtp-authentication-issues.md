---
title: Ativar a autenticação e reação de problemas SMTP
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 4695a2f111823739c4d87fa2b262a5e64e080955
ms.sourcegitcommit: 2103d706492ad7ee9596344714c0520569ebd6af
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/23/2021
ms.locfileid: "53077662"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a><span data-ttu-id="ac045-102">Ativar a autenticação e reação de problemas SMTP</span><span class="sxs-lookup"><span data-stu-id="ac045-102">Enable SMTP authentication and troubleshooting</span></span>

<span data-ttu-id="ac045-103">Se quiser ativar a autenticação SMTP para uma caixa de correio ou se estiver a obter um "Cliente não autenticado", Erro "Autenticação sem sucesso" ou "SmtpClientAuthentication" com o código 5.7.57 ou 5.7.3 ou 5.7.139 quando tenta reenviar o e-mail ao autenticar um dispositivo ou aplicação com o Microsoft 365, efetue estas três ações para resolver o problema:</span><span class="sxs-lookup"><span data-stu-id="ac045-103">If you want to enable SMTP authentication for a mailbox or you're getting a "Client not authenticated", "Authentication unsuccessful", or "SmtpClientAuthentication" error with code 5.7.57 or 5.7.3 or 5.7.139 when you try to relay email by authenticating a device or application with Microsoft 365, perform these three actions to resolve the issue:</span></span>

1. <span data-ttu-id="ac045-104">Desativar as [predefinições de](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) segurança do Azure ao ativar as **predefinições de segurança** para **Não.**</span><span class="sxs-lookup"><span data-stu-id="ac045-104">Disable the [Azure security defaults](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) by toggling **Enable security defaults** to **No**.</span></span>

    <span data-ttu-id="ac045-105">a.</span><span class="sxs-lookup"><span data-stu-id="ac045-105">a.</span></span> <span data-ttu-id="ac045-106">Inscreva-se no portal do Azure como administrador de segurança, administrador de Acesso Condicional ou administrador global.</span><span class="sxs-lookup"><span data-stu-id="ac045-106">Sign in to the Azure portal as a Security administrator, Conditional Access administrator, or global administrator.</span></span><BR/>
    <span data-ttu-id="ac045-107">b.</span><span class="sxs-lookup"><span data-stu-id="ac045-107">b.</span></span> <span data-ttu-id="ac045-108">Navegue até Azure Active Directory > **Propriedades.**</span><span class="sxs-lookup"><span data-stu-id="ac045-108">Browse to Azure Active Directory > **Properties**.</span></span><BR/>
    <span data-ttu-id="ac045-109">c.</span><span class="sxs-lookup"><span data-stu-id="ac045-109">c.</span></span> <span data-ttu-id="ac045-110">**Selecione Gerir predefinições de segurança**.</span><span class="sxs-lookup"><span data-stu-id="ac045-110">Select **Manage security defaults**.</span></span><BR/>
    <span data-ttu-id="ac045-111">d.</span><span class="sxs-lookup"><span data-stu-id="ac045-111">d.</span></span> <span data-ttu-id="ac045-112">Defina **Ativar as predefinições** de **segurança para Não**.</span><span class="sxs-lookup"><span data-stu-id="ac045-112">Set **Enable security defaults** to **No**.</span></span><BR/>
    <span data-ttu-id="ac045-113">e.</span><span class="sxs-lookup"><span data-stu-id="ac045-113">e.</span></span> <span data-ttu-id="ac045-114">Seleccione **Guardar**.</span><span class="sxs-lookup"><span data-stu-id="ac045-114">Select **Save**.</span></span>

2. <span data-ttu-id="ac045-115">[Ative a submissão SMTP de](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) Cliente na caixa de correio licenciada.</span><span class="sxs-lookup"><span data-stu-id="ac045-115">[Enable Client SMTP submission](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) on the licensed mailbox.</span></span>

    <span data-ttu-id="ac045-116">a.</span><span class="sxs-lookup"><span data-stu-id="ac045-116">a.</span></span> <span data-ttu-id="ac045-117">A partir do centro de administração do Microsoft 365, vá para Utilizadores **Ativos** e selecione o utilizador.</span><span class="sxs-lookup"><span data-stu-id="ac045-117">From the Microsoft 365 admin center, go to **Active Users**, and select the user.</span></span><BR/>
    <span data-ttu-id="ac045-118">b.</span><span class="sxs-lookup"><span data-stu-id="ac045-118">b.</span></span> <span data-ttu-id="ac045-119">Vá para o separador Correio e, em Aplicações **de e-mail**, selecione **Gerir aplicações de e-mail**.</span><span class="sxs-lookup"><span data-stu-id="ac045-119">Go to Mail tab, and under **Email apps**, select **Manage email apps**.</span></span><BR/>
    <span data-ttu-id="ac045-120">d.</span><span class="sxs-lookup"><span data-stu-id="ac045-120">d.</span></span> <span data-ttu-id="ac045-121">Certifique-se **de que O SMTP Autenticado** está se des marcada (ativado).</span><span class="sxs-lookup"><span data-stu-id="ac045-121">Make sure **Authenticated SMTP** is checked (enabled).</span></span><BR/>
    <span data-ttu-id="ac045-122">e.</span><span class="sxs-lookup"><span data-stu-id="ac045-122">e.</span></span> <span data-ttu-id="ac045-123">**Selecione Guardar alterações**.</span><span class="sxs-lookup"><span data-stu-id="ac045-123">Select **Save changes**.</span></span><BR/>

3. <span data-ttu-id="ac045-124">[Desativar a Autenticação Multifatores (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) na caixa de correio licenciada.</span><span class="sxs-lookup"><span data-stu-id="ac045-124">[Disable Multi-Factor Authentication (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) on the licensed mailbox.</span></span>

    <span data-ttu-id="ac045-125">a.</span><span class="sxs-lookup"><span data-stu-id="ac045-125">a.</span></span> <span data-ttu-id="ac045-126">Vá para o centro de administração do Microsoft 365 e, no menu de navegação esquerdo, selecione **Utilizadores**  >  **Ativos.**</span><span class="sxs-lookup"><span data-stu-id="ac045-126">Go to the Microsoft 365 admin center, and in the left navigation menu select **Users** > **Active users**.</span></span><BR/>
    <span data-ttu-id="ac045-127">b.</span><span class="sxs-lookup"><span data-stu-id="ac045-127">b.</span></span> <span data-ttu-id="ac045-128">**Selecione Autenticação multifator.**</span><span class="sxs-lookup"><span data-stu-id="ac045-128">Select **Multi-factor authentication**.</span></span><BR/>
    <span data-ttu-id="ac045-129">c.</span><span class="sxs-lookup"><span data-stu-id="ac045-129">c.</span></span> <span data-ttu-id="ac045-130">Selecione o utilizador e **desativar a austeridade Multifator.**</span><span class="sxs-lookup"><span data-stu-id="ac045-130">Select the user and disable **Multi-Factor auth**.</span></span><BR/>
