---
title: Papel privilegiado de Gestão de Identidade
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
- "9003230"
- "6825"
ms.openlocfilehash: 726511d016462f56c48a4272b57abc3e9f0cbc3d
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088876"
---
# <a name="privileged-identity-managementpim-role"></a><span data-ttu-id="0f9ac-102">Papel privilegiado de Gestão de Identidade (PIM)</span><span class="sxs-lookup"><span data-stu-id="0f9ac-102">Privileged Identity Management(PIM) role</span></span>

<span data-ttu-id="0f9ac-103">**As permissões não são concedidas após a ativação de uma função**</span><span class="sxs-lookup"><span data-stu-id="0f9ac-103">**Permissions are not granted after activating a role**</span></span>

<span data-ttu-id="0f9ac-104">Quando ativar uma função na Gestão de Identidade Privilegiada AD Azure (PIM), a ativação pode não se propagar instantaneamente a todos os portais que requerem o papel privilegiado.</span><span class="sxs-lookup"><span data-stu-id="0f9ac-104">When you activate a role in Azure AD Privileged Identity Management (PIM), the activation may not instantly propagate to all portals that require the privileged role.</span></span> <span data-ttu-id="0f9ac-105">Por vezes, mesmo que a mudança seja propagada, o caching web num portal pode resultar na alteração não ter efeito imediatamente.</span><span class="sxs-lookup"><span data-stu-id="0f9ac-105">Sometimes, even if the change is propagated, web caching in a portal may result in the change not taking effect immediately.</span></span>

<span data-ttu-id="0f9ac-106">Se a sua ativação for retardada, siga estes passos:</span><span class="sxs-lookup"><span data-stu-id="0f9ac-106">If your activation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="0f9ac-107">Assine fora do portal Azure e depois volte a entrar.</span><span class="sxs-lookup"><span data-stu-id="0f9ac-107">Sign out of the Azure portal and then sign back in.</span></span> <span data-ttu-id="0f9ac-108">Quando ativar uma função AD Azure ou uma função de recurso Azure, verá as fases da sua ativação.</span><span class="sxs-lookup"><span data-stu-id="0f9ac-108">When you activate an Azure AD role or an Azure resource role, you will see the stages of your activation.</span></span> <span data-ttu-id="0f9ac-109">Uma vez concluídas todas as etapas, verá um link 'Sign out'.</span><span class="sxs-lookup"><span data-stu-id="0f9ac-109">Once all the stages are complete, you will see a 'Sign out' link.</span></span> <span data-ttu-id="0f9ac-110">Pode usar este link para assinar. Isto resolverá a maioria dos casos para atraso de ativação.</span><span class="sxs-lookup"><span data-stu-id="0f9ac-110">You can use this link to sign out. This will solve most cases for activation delay.</span></span>
2. <span data-ttu-id="0f9ac-111">Na PIM, verifique se está listado como membro do papel.</span><span class="sxs-lookup"><span data-stu-id="0f9ac-111">In PIM, verify that you are listed as the member of the role.</span></span>
3. <span data-ttu-id="0f9ac-112">Se estiver a ativar a função de Administrador de Troca, certifique-se de que assina e volta a entrar.</span><span class="sxs-lookup"><span data-stu-id="0f9ac-112">If you are activating the Exchange Administrator role, make sure you sign out and sign back in.</span></span> <span data-ttu-id="0f9ac-113">Se o problema persistir, abra um bilhete de apoio e levante-o como um problema.</span><span class="sxs-lookup"><span data-stu-id="0f9ac-113">If the problem persists, open a support ticket and raise this as an issue.</span></span> <span data-ttu-id="0f9ac-114">Se estiver a utilizar a sua função de Administrador de Intercâmbio para aceder ao Centro de Segurança e Conformidade, consulte o próximo passo.</span><span class="sxs-lookup"><span data-stu-id="0f9ac-114">If you are using your Exchange Administrator role to access the Security and Compliance Center, see the next step.</span></span>
4. <span data-ttu-id="0f9ac-115">Se estiver a ativar uma função para aceder ao Centro de Segurança e Conformidade ou se estiver a ativar a função de Administrador SharePoint, sentirá algum atraso de ativação de alguns minutos até algumas horas.</span><span class="sxs-lookup"><span data-stu-id="0f9ac-115">If you are activating a role to access the Security and Compliance Center or if you are activating the SharePoint Administrator role, you will experience some activation delay from a few minutes up to a few hours.</span></span> <span data-ttu-id="0f9ac-116">Esta é uma questão conhecida e estamos a trabalhar ativamente com estas equipas para resolver esta questão o mais rapidamente possível.</span><span class="sxs-lookup"><span data-stu-id="0f9ac-116">This is a known issue and we are actively working with these teams to resolve this issue as soon as possible.</span></span>

<span data-ttu-id="0f9ac-117">Para obter mais informações, consulte:</span><span class="sxs-lookup"><span data-stu-id="0f9ac-117">For more information, see:</span></span>

- [<span data-ttu-id="0f9ac-118">Ativar os meus papéis de AD Azure em PIM</span><span class="sxs-lookup"><span data-stu-id="0f9ac-118">Activate my Azure AD roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [<span data-ttu-id="0f9ac-119">Ativar os meus papéis de recurso Azure na PIM</span><span class="sxs-lookup"><span data-stu-id="0f9ac-119">Activate my Azure resource roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

<span data-ttu-id="0f9ac-120">**As permissões não são removidas após desativar uma função ou a ativação da função expira**</span><span class="sxs-lookup"><span data-stu-id="0f9ac-120">**Permissions are not removed after deactivating a role or the role activation expires**</span></span>

<span data-ttu-id="0f9ac-121">Quando desativa um papel na Gestão de Identidade Privilegiada AD Azure ou quando um período de ativação de funções expirar, pode haver um atraso onde continua a ter acesso.</span><span class="sxs-lookup"><span data-stu-id="0f9ac-121">When you deactivate a role in Azure AD Privileged Identity Management or when a role activation period expires, there might be a delay where you continue to have access.</span></span>

<span data-ttu-id="0f9ac-122">Se a sua desativação for adiada, siga estes passos:</span><span class="sxs-lookup"><span data-stu-id="0f9ac-122">If your deactivation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="0f9ac-123">Se estiver a desativar a função de Administrador de Câmbio ou o período de ativação da função expirar, e notar um atraso significativo antes de as permissões serem removidas, abra um bilhete de apoio e diga ao seu engenheiro de suporte para o ajudar a arquivar um bilhete com a equipa de Gestão de Acesso Privilegiado (PAM) dentro do Office sobre este assunto.</span><span class="sxs-lookup"><span data-stu-id="0f9ac-123">If you are deactivating the Exchange Administrator role or the role activation period expires, and you notice a significant delay before the permissions are removed, open a support ticket and tell your support engineer to help you file a ticket with the Privileged Access Management (PAM) team inside Office about this issue.</span></span>
2. <span data-ttu-id="0f9ac-124">Se o período de ativação tiver expirado, mas ainda tiver a sessão do navegador aberta, feche o seu navegador.</span><span class="sxs-lookup"><span data-stu-id="0f9ac-124">If the activation period has expired, but you still have the browser session open, close your browser.</span></span> <span data-ttu-id="0f9ac-125">Pode continuar a usar o papel até encerrar a sessão.</span><span class="sxs-lookup"><span data-stu-id="0f9ac-125">You can continue to use the role until you close that session.</span></span> <span data-ttu-id="0f9ac-126">Esta é uma questão conhecida e estamos a estudar uma possível correção para revogar ativamente cada sessão uma vez expirada a ativação.</span><span class="sxs-lookup"><span data-stu-id="0f9ac-126">This is a known issue and we are looking at a potential fix to actively revoke each session once activation has expired.</span></span>

<span data-ttu-id="0f9ac-127">Se o seu atraso for diferente destes dois cenários, por favor abra um bilhete de apoio.</span><span class="sxs-lookup"><span data-stu-id="0f9ac-127">If your delay is different than these two scenarios, please open a support ticket.</span></span>
