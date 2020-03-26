---
title: Não é possível iniciar sessão no Teams devido ao erro autologon.microsoftazuread-sso.com:443
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 77049153939989d1c63789adfec0b494d047a6e4
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932035"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a><span data-ttu-id="eeb93-102">Não é possível iniciar sessão no Teams devido ao erro autologon.microsoftazuread-sso dot com:443</span><span class="sxs-lookup"><span data-stu-id="eeb93-102">Unable to log into Teams due to error autologon.microsoftazuread-sso dot com:443</span></span>

<span data-ttu-id="eeb93-103">Se o SSO Totalmente Integrado estiver ativado como autenticação do O365, o URL "autologon.microsoftazuread-sso.com" poderá ter de ser adicionado aos Sites da Intranet.</span><span class="sxs-lookup"><span data-stu-id="eeb93-103">If Seamless SSO is enabled as the O365 authentication, the URL "autologon.microsoftazuread-sso.com" may need to be added to Intranet Sites.</span></span>  <span data-ttu-id="eeb93-104">Se este tiver sido adicionado anteriormente aos Sites Fidedignos e se o SSO Totalmente Integrado estiver a ser utilizado, deverá ser removido dos Sites Fidedignos.</span><span class="sxs-lookup"><span data-stu-id="eeb93-104">If it has previously been added to Trusted Sites  and Seamless SSO is in use, it should be removed from Trusted Sites.</span></span>

<span data-ttu-id="eeb93-105">Consulte a [Lista de Verificação de Problemas com o SSO Troubleshooting Checklist](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).</span><span class="sxs-lookup"><span data-stu-id="eeb93-105">Please review the [Seamless SSO Troubleshooting Checklist](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).</span></span>

<span data-ttu-id="eeb93-106">Siga estes passos para adicionar um URL à lista de Sites intranet:</span><span class="sxs-lookup"><span data-stu-id="eeb93-106">Follow these steps to add a URL to Intranet Sites list:</span></span>

1. <span data-ttu-id="eeb93-107">Abra o Internet Explorer ao clicar no botão **Iniciar**.</span><span class="sxs-lookup"><span data-stu-id="eeb93-107">Open Internet Explorer by clicking the **Start** button.</span></span> <span data-ttu-id="eeb93-108">Na caixa de pesquisa, escreva Internet Explorer e, em seguida, na lista de resultados, clique **Internet Explorer**.</span><span class="sxs-lookup"><span data-stu-id="eeb93-108">In the search box, type Internet Explorer, and then, in the list of results, click **Internet Explorer**.</span></span>
2. <span data-ttu-id="eeb93-109">Clique em **Ferramentas** e, em seguida, clique em **opções de Internet**.</span><span class="sxs-lookup"><span data-stu-id="eeb93-109">Click **Tools**, and then click **Internet options**.</span></span>
3. <span data-ttu-id="eeb93-110">Clique no separador **Segurança**.</span><span class="sxs-lookup"><span data-stu-id="eeb93-110">Click the **Security** tab.</span></span>
4. <span data-ttu-id="eeb93-111">Agora, clique em **sites da Intranet Local**, em seguida, no botão **sites** e, finalmente, no botão **Avançadas**.</span><span class="sxs-lookup"><span data-stu-id="eeb93-111">Now click on **Local Intranet sites** and then click on the **sites** button and then **Advanced** button.</span></span>
5. <span data-ttu-id="eeb93-112">Introduza o URL do Site e clique em **Adicionar**.</span><span class="sxs-lookup"><span data-stu-id="eeb93-112">Enter the Website URL and click **Add**.</span></span>
6. <span data-ttu-id="eeb93-113">Quando terminar, clique em **Fechar**.</span><span class="sxs-lookup"><span data-stu-id="eeb93-113">When you are finished, click **Close**.</span></span>

<span data-ttu-id="eeb93-114">Para mais informações, consulte [Documentação para a implementação de SSO Totalmente Integrado para o O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (inclui processo baseado em Políticas para adicionar um URL aos Sites Intranet no passo 3).</span><span class="sxs-lookup"><span data-stu-id="eeb93-114">For more information, see [Documentation for deploying Seamless SSO for O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (includes Policy-based process to add a URL to Intranet Sites in Step 3).</span></span>
