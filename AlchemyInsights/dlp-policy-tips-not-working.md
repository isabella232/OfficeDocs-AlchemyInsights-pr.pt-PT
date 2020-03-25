---
title: Dicas políticas dlp não funcionam
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 51b4472fa721443192eb542cac45965df67634df
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932597"
---
# <a name="dlp-policy-tip-issues"></a><span data-ttu-id="98090-102">DLP Questões de Ponta Política</span><span class="sxs-lookup"><span data-stu-id="98090-102">DLP Policy Tip issues</span></span>

<span data-ttu-id="98090-103">**Importante**: Muitos clientes SharePoint Online e OneDrive executam aplicações críticas ao negócio contra o serviço que executa em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="98090-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="98090-104">Estes incluem migração de conteúdos, Prevenção de Perdas de Dados (DLP) e soluções de backup.</span><span class="sxs-lookup"><span data-stu-id="98090-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="98090-105">Durante estes tempos sem precedentes, estamos a tomar medidas para garantir que os serviços SharePoint Online e OneDrive permanecem altamente disponíveis e fiáveis para os seus utilizadores que dependem mais do serviço do que nunca em cenários de trabalho remoto.</span><span class="sxs-lookup"><span data-stu-id="98090-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="98090-106">Em apoio a este objetivo, implementámos limites de estrangulamento mais apertados em aplicações de fundo (soluções de migração, DLP e backup) durante o dia da semana.</span><span class="sxs-lookup"><span data-stu-id="98090-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="98090-107">Deve esperar que estas aplicações atinjam uma entrada muito limitada durante estes tempos.</span><span class="sxs-lookup"><span data-stu-id="98090-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="98090-108">No entanto, durante as horas de noite e fim de semana para a região, o serviço estará pronto para processar um volume significativamente maior de pedidos de aplicações de fundo.</span><span class="sxs-lookup"><span data-stu-id="98090-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="98090-109">**Dicas políticas dlp**</span><span class="sxs-lookup"><span data-stu-id="98090-109">**DLP policy tips**</span></span>

<span data-ttu-id="98090-110">Ao utilizar **as políticas dLP,** os utilizadores podem ser notificados de uma violação de política com dicas de **política.**</span><span class="sxs-lookup"><span data-stu-id="98090-110">When using **DLP policies**, users can be notified of a policy violation with **policy tips**.</span></span> <span data-ttu-id="98090-111">Os administradores podem configurar dicas de política para exibir enquanto testam a sua política dLP ou quando a política está em pleno modo de execução.</span><span class="sxs-lookup"><span data-stu-id="98090-111">Admins can configure policy tips to display while testing their DLP policy or when the policy is in full enforcement mode.</span></span>
  
<span data-ttu-id="98090-112">Para configurar as dicas de política na sua política dLP no centro de segurança e conformidade em modo de execução completo, faça o seguinte:</span><span class="sxs-lookup"><span data-stu-id="98090-112">To configure policy tips on your DLP policy in the Security and Compliance center in full enforcement mode, do the following:</span></span>
  
- <span data-ttu-id="98090-113">Certifique-se de que as dicas de política foram **ativadas** na regra DLP utilizando os passos [aqui .](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="98090-113">Ensure policy tips have been **enabled** on the DLP rule using the steps [here](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span></span>

- <span data-ttu-id="98090-114">Certifique-se de que o seu **conteúdo corresponde** ao **necessário** para desencadear a regra descrita neste artigo [aqui](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="98090-114">Ensure your **content matches** what is **required** to trigger the rule outlined in this article [here](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="98090-115">Exibição de dicas de política tanto no OWA como no Outlook.</span><span class="sxs-lookup"><span data-stu-id="98090-115">Policy tips display in both OWA and Outlook.</span></span> <span data-ttu-id="98090-116">No entanto, ao utilizar **o Outlook 2013 ou mais tarde,** as dicas de política só são apresentadas em determinadas condições.</span><span class="sxs-lookup"><span data-stu-id="98090-116">However, when using **Outlook 2013 or later**, policy tips are only displayed under certain conditions.</span></span> <span data-ttu-id="98090-117">Estas condições estão listadas aqui: [Condições suportadas para o Outlook 2013 ou mais tarde para exibir Dicas](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions) políticas</span><span class="sxs-lookup"><span data-stu-id="98090-117">These conditions are listed here: [Supported conditions for Outlook 2013 or later for displaying Policy Tips](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span></span>

<span data-ttu-id="98090-118">Para obter informações adicionais sobre as dicas políticas do DLP, consulte: [Mostrar dicas políticas para políticas de DLP](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="98090-118">For additional information on DLP policy tips, see: [Show policy tips for DLP Policies](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span></span>
  