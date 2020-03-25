---
title: Mais informações sobre questões dlp
ms.author: pebaum
author: pebaum
manager: laurawi
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2447"
- "3200001"
ms.openlocfilehash: 6525cee0555f1ae67b7d4e32445b9a1537d4a804
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932705"
---
# <a name="information-about-dlp-issues"></a><span data-ttu-id="9ca01-102">Informação sobre questões dlp</span><span class="sxs-lookup"><span data-stu-id="9ca01-102">Information about DLP issues</span></span>

<span data-ttu-id="9ca01-103">**Importante**: Muitos clientes SharePoint Online e OneDrive executam aplicações críticas ao negócio contra o serviço que executa em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="9ca01-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="9ca01-104">Estes incluem migração de conteúdos, Prevenção de Perdas de Dados (DLP) e soluções de backup.</span><span class="sxs-lookup"><span data-stu-id="9ca01-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="9ca01-105">Durante estes tempos sem precedentes, estamos a tomar medidas para garantir que os serviços SharePoint Online e OneDrive permanecem altamente disponíveis e fiáveis para os seus utilizadores que dependem mais do serviço do que nunca em cenários de trabalho remoto.</span><span class="sxs-lookup"><span data-stu-id="9ca01-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="9ca01-106">Em apoio a este objetivo, implementámos limites de estrangulamento mais apertados em aplicações de fundo (soluções de migração, DLP e backup) durante o dia da semana.</span><span class="sxs-lookup"><span data-stu-id="9ca01-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="9ca01-107">Deve esperar que estas aplicações atinjam uma entrada muito limitada durante estes tempos.</span><span class="sxs-lookup"><span data-stu-id="9ca01-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="9ca01-108">No entanto, durante as horas de noite e fim de semana para a região, o serviço estará pronto para processar um volume significativamente maior de pedidos de aplicações de fundo.</span><span class="sxs-lookup"><span data-stu-id="9ca01-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="9ca01-109">**Informação sobre a política do DLP**</span><span class="sxs-lookup"><span data-stu-id="9ca01-109">**Information on DLP policy**</span></span>

<span data-ttu-id="9ca01-110">Com uma política dLP, pode identificar, monitorizar e proteger automaticamente informações sensíveis através do Office 365.</span><span class="sxs-lookup"><span data-stu-id="9ca01-110">With a DLP policy, you can identify, monitor, and automatically protect sensitive information across Office 365.</span></span>

<span data-ttu-id="9ca01-111">Visite estes links para mais informações:</span><span class="sxs-lookup"><span data-stu-id="9ca01-111">Please visit these links for more information:</span></span>

- [<span data-ttu-id="9ca01-112">Visão geral da prevenção da perda de dados</span><span class="sxs-lookup"><span data-stu-id="9ca01-112">Overview of data loss prevention</span></span>](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies)
- [<span data-ttu-id="9ca01-113">O que os tipos de informação sensíveis procuram</span><span class="sxs-lookup"><span data-stu-id="9ca01-113">What the sensitive information types look for</span></span>](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
- [<span data-ttu-id="9ca01-114">Criar um tipo de informação sensível personalizado</span><span class="sxs-lookup"><span data-stu-id="9ca01-114">Create a custom sensitive information type</span></span>](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type)
- [<span data-ttu-id="9ca01-115">Envie notificações de e-mail e mostre dicas de política</span><span class="sxs-lookup"><span data-stu-id="9ca01-115">Send email notifications and show policy tips</span></span>](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)
- [<span data-ttu-id="9ca01-116">Proteja ficheiros Online SharePoint com etiquetas de retenção e DLP</span><span class="sxs-lookup"><span data-stu-id="9ca01-116">Protect SharePoint Online files with retention labels and DLP</span></span>](https://docs.microsoft.com/office365/securitycompliance/protect-sharepoint-online-files-with-office-365-labels-and-dlp)
- [<span data-ttu-id="9ca01-117">Equipas DLP e Microsoft</span><span class="sxs-lookup"><span data-stu-id="9ca01-117">DLP and Microsoft Teams</span></span>](https://docs.microsoft.com/office365/securitycompliance/dlp-microsoft-teams)

<span data-ttu-id="9ca01-118">Para testar os seus dados com um tipo de informação sensível incorporada ou personalizada, utilize a opção **do tipo Teste** em tipos de**informação sensíveis**de **classificações** > .</span><span class="sxs-lookup"><span data-stu-id="9ca01-118">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="9ca01-119">Para mais informações, consulte os tipos de [informação personalizadas](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="9ca01-119">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>