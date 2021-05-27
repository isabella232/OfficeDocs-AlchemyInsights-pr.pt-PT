---
title: Os indicadores não funcionam com o browser Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11230"
- "9005470"
ms.openlocfilehash: df62d965e0dc2ddb656571af99b1e4c3cb52ea35
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676463"
---
# <a name="indicators-dont-work-using-edge-browser"></a><span data-ttu-id="0a3a9-102">Os indicadores não funcionam com o browser Edge</span><span class="sxs-lookup"><span data-stu-id="0a3a9-102">Indicators don't work using Edge browser</span></span>

<span data-ttu-id="0a3a9-103">Depois de criar um Indicador, este não é honrado pelo Edge (Smartscreen).</span><span class="sxs-lookup"><span data-stu-id="0a3a9-103">After you created an Indicator, it's not honored by Edge (Smartscreen).</span></span> <span data-ttu-id="0a3a9-104">Para obter mais informações, [consulte Criar indicadores para IPs e URLs/domínios.](/microsoft-365/security/defender-endpoint/indicator-ip-domain)</span><span class="sxs-lookup"><span data-stu-id="0a3a9-104">For more information, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>

## <a name="step-1-ensure-the-following"></a><span data-ttu-id="0a3a9-105">Passo 1: certifique-se de que o seguinte</span><span class="sxs-lookup"><span data-stu-id="0a3a9-105">Step 1: Ensure the following</span></span>

- <span data-ttu-id="0a3a9-106">Verifique se o indicador está correto (sem erros de digitação em IP/URL, a ação correta, os grupos RBAC corretos).</span><span class="sxs-lookup"><span data-stu-id="0a3a9-106">Verify that the indicator is correct (no typos in IP/URL, correct action, the correct RBAC groups).</span></span>
- <span data-ttu-id="0a3a9-107">Aguarde pelo menos 2 horas após criar o indicador para ter em conta qualquer latência possível.</span><span class="sxs-lookup"><span data-stu-id="0a3a9-107">Wait the minimum 2 hours after creating the indicator to take into account any possible latency.</span></span>
- <span data-ttu-id="0a3a9-108">Confirme que o(s) sistema(s) está ativo(s) no Microsoft Defender para Endpoint.</span><span class="sxs-lookup"><span data-stu-id="0a3a9-108">Confirm that the system(s) are onboarded to Microsoft Defender for Endpoint.</span></span>
- <span data-ttu-id="0a3a9-109">Verifique se o(s) sistema(s) pode comunicar com a Nuvem.</span><span class="sxs-lookup"><span data-stu-id="0a3a9-109">Verify that system(s) can communicate with the Cloud.</span></span>
- <span data-ttu-id="0a3a9-110">Verifique se o Smartscreen está ativado e acessível ao ir para o [site de teste.](https://demo.smartscreen.msft.net)</span><span class="sxs-lookup"><span data-stu-id="0a3a9-110">Verify that Smartscreen is enabled and reachable by going to the [test site](https://demo.smartscreen.msft.net).</span></span>

## <a name="step-2-troubleshoot-the-potential-issue"></a><span data-ttu-id="0a3a9-111">Passo 2: remoção do possível problema</span><span class="sxs-lookup"><span data-stu-id="0a3a9-111">Step 2: Troubleshoot the potential issue</span></span>

- <span data-ttu-id="0a3a9-112">Certifique-se de que o cliente cumpre os requisitos.</span><span class="sxs-lookup"><span data-stu-id="0a3a9-112">Make sure the client meets the requirements.</span></span> <span data-ttu-id="0a3a9-113">Para obter detalhes, [consulte Criar indicadores para IPs e URLs/domínios.](/microsoft-365/security/defender-endpoint/indicator-ip-domain)</span><span class="sxs-lookup"><span data-stu-id="0a3a9-113">For details, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>
- <span data-ttu-id="0a3a9-114">Certifique-se de que está a executar a versão mais recente do browser Edge.</span><span class="sxs-lookup"><span data-stu-id="0a3a9-114">Make sure you're running the latest version of the Edge browser.</span></span> <span data-ttu-id="0a3a9-115">Para saber qual é a versão mais recente, [consulte Saber que versão do Microsoft Edge que tem.](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb)</span><span class="sxs-lookup"><span data-stu-id="0a3a9-115">To find out the latest version, see [Find out which version of Microsoft Edge you have](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).</span></span>
- <span data-ttu-id="0a3a9-116">Reinicie o browser Edge.</span><span class="sxs-lookup"><span data-stu-id="0a3a9-116">Restart the Edge browser.</span></span>
- <span data-ttu-id="0a3a9-117">Navegue para o site para o qual tem um indicador de configuração.</span><span class="sxs-lookup"><span data-stu-id="0a3a9-117">Navigate to the site for which you have setup an indicator.</span></span> <span data-ttu-id="0a3a9-118">Se o site não aparecer como esperado, continue para o Passo 3.</span><span class="sxs-lookup"><span data-stu-id="0a3a9-118">If the site does not appear as expected, continue to Step 3.</span></span> 

## <a name="step-3-collect-data"></a><span data-ttu-id="0a3a9-119">Passo 3: recolher dados</span><span class="sxs-lookup"><span data-stu-id="0a3a9-119">Step 3: Collect data</span></span>

- <span data-ttu-id="0a3a9-120">Recolha **dados de diagnóstico do MDEClientAnalyzer.**</span><span class="sxs-lookup"><span data-stu-id="0a3a9-120">Collect **MDEClientAnalyzer** diagnostic data.</span></span> <span data-ttu-id="0a3a9-121">Para obter instruções, consulte [Problemas com máquinas de iboard no Microsoft Defender para Endpoint.](issues-with-onboarding-machines.md)</span><span class="sxs-lookup"><span data-stu-id="0a3a9-121">For instructions, see [Issues with onboarding machines to Microsoft Defender for Endpoint](issues-with-onboarding-machines.md).</span></span>
- <span data-ttu-id="0a3a9-122">Se estiver à vontade a instalar e a recolher um rastreio Do Fiddler, consulte [Telerik Fiddler.](http://www.telerik.com/fiddler)</span><span class="sxs-lookup"><span data-stu-id="0a3a9-122">If you are comfortable installing and collecting a Fiddler trace, see [Telerik Fiddler](http://www.telerik.com/fiddler).</span></span>
- <span data-ttu-id="0a3a9-123">Se preferir orientação do Suporte da Microsoft, selecione o ícone de Suporte abaixo para abrir um caso de suporte.</span><span class="sxs-lookup"><span data-stu-id="0a3a9-123">If you prefer guidance from Microsoft Support, select the Support icon below to open a support case.</span></span>
