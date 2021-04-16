---
title: Introdução aos evento em direto no Microsoft Teams
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
- "9000208"
- "3436"
ms.openlocfilehash: a10f756fc69a7a135446d8d3bcec1f5e951627d8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51811971"
---
# <a name="getting-started-with-teams-live-events"></a><span data-ttu-id="eeca1-102">Introdução aos evento em direto no Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="eeca1-102">Getting started with Teams live events</span></span>

<span data-ttu-id="eeca1-103">Os eventos em direto do Microsoft Teams são uma extensão das reuniões do Teams que lhe permitem agendar e produzir eventos que são transmitidos para vastos públicos online.</span><span class="sxs-lookup"><span data-stu-id="eeca1-103">Microsoft Teams live events are an extension of Teams meetings that enable you to schedule and produce events that stream to large online audiences.</span></span>

<span data-ttu-id="eeca1-104">Para criar um evento em direto, precisará do seguinte:</span><span class="sxs-lookup"><span data-stu-id="eeca1-104">To create a live event, you will need the following:</span></span>

- <span data-ttu-id="eeca1-105">Em primeiro lugar, confirme se os eventos do Teams em direto estão [disponíveis no seu país/região](https://docs.microsoft.com/microsoftteams/teams-live-events/plan-for-teams-live-events#regional-availability); os eventos em direto ainda não são suportados em alguns países.</span><span class="sxs-lookup"><span data-stu-id="eeca1-105">First, confirm that Teams Live Events are [available in your Country and Region](https://docs.microsoft.com/microsoftteams/teams-live-events/plan-for-teams-live-events#regional-availability); Live Events are not yet supported in some countries.</span></span>  <span data-ttu-id="eeca1-106">Se atribuiu licenças e configurou políticas, mas ainda não consegue criar um evento do Teams em direto, é provável que esteja num país/região onde os eventos em direto ainda não estão disponíveis.</span><span class="sxs-lookup"><span data-stu-id="eeca1-106">If you’ve assigned licenses and set policies, but still cannot create a Teams Live Event, it is likely you are in a Country or Region where Live Events is not yet available.</span></span>

- <span data-ttu-id="eeca1-107">Uma [licença do Office 365 Enterprise E1, E3, ou E5 ou uma licença do Office 365 A3 ou A5](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#step-2-get-and-assign-licenses).</span><span class="sxs-lookup"><span data-stu-id="eeca1-107">An [Office 365 Enterprise E1, E3, or E5 license or an Office 365 A3 or A5 license](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#step-2-get-and-assign-licenses).</span></span> <span data-ttu-id="eeca1-108">**Nota**: devido a um recente aumento de utilização do Teams, ao atribuir uma licença do Teams a um utilizador, poderá ter de aguardar cerca de 24 horas até que a configuração esteja completa.</span><span class="sxs-lookup"><span data-stu-id="eeca1-108">**Note**: Due to a recent increase in Teams usage, when you assign a Teams license to a user, it may take around 24 hours before they'll be fully set up.</span></span> <span data-ttu-id="eeca1-109">Até isso acontecer, não poderá atribuir-lhes políticas do Teams, e é possível que os utilizadores não tenham acesso a algumas funcionalidades do Teams, como chamadas e conferências de áudio.</span><span class="sxs-lookup"><span data-stu-id="eeca1-109">Until then, you won't be able to assign Teams policies to them, and they might not have access to some Teams features like calling and audio conferencing.</span></span>

- <span data-ttu-id="eeca1-110">Permissão para [criar eventos em direito no centro de administração do Microsoft Teams](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#create-or-edit-a-live-events-policy).</span><span class="sxs-lookup"><span data-stu-id="eeca1-110">Permission to [create live events in Microsoft Teams admin center](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#create-or-edit-a-live-events-policy).</span></span>

- <span data-ttu-id="eeca1-111">Permissão para [criar eventos ao vivo no Microsoft Stream](https://docs.microsoft.com/microsoftteams/teams-live-events/what-are-teams-live-events) (para eventos produzidos com recurso a uma aplicação ou dispositivo de transmissão externo).</span><span class="sxs-lookup"><span data-stu-id="eeca1-111">Permission to [create live events in Microsoft Stream](https://docs.microsoft.com/microsoftteams/teams-live-events/what-are-teams-live-events) (for events produced using an external broadcasting app or device).</span></span>

- <span data-ttu-id="eeca1-112">Ter uma associação completa à organização (não pode ser um convidado ou de outra organização).</span><span class="sxs-lookup"><span data-stu-id="eeca1-112">Full team membership in the org (can't be a guest or from another org).</span></span>
<span data-ttu-id="eeca1-113">Agendamento de reuniões privadas, partilha de ecrãs e partilha de vídeo IP, ter ativado a política de reunião do Teams.</span><span class="sxs-lookup"><span data-stu-id="eeca1-113">Private meeting scheduling, screensharing, and IP video sharing, turned on in Team meeting policy.</span></span>

- <span data-ttu-id="eeca1-114">[Melhores práticas](https://support.office.com/article/Best-practices-for-producing-a-Teams-live-event-e500370e-4dd1-4187-8b48-af10ef02cf42) para eventos em direto do Teams.</span><span class="sxs-lookup"><span data-stu-id="eeca1-114">[Best practices](https://support.office.com/article/Best-practices-for-producing-a-Teams-live-event-e500370e-4dd1-4187-8b48-af10ef02cf42) for Teams Live Events.</span></span>

<span data-ttu-id="eeca1-115">Para mais informações, consulte [Introdução aos evento em direto no Microsoft Teams](https://support.office.com/article/get-started-with-microsoft-teams-live-events-d077fec2-a058-483e-9ab5-1494afda578a).</span><span class="sxs-lookup"><span data-stu-id="eeca1-115">For more information, please see [Get started with Microsoft Teams live events](https://support.office.com/article/get-started-with-microsoft-teams-live-events-d077fec2-a058-483e-9ab5-1494afda578a).</span></span>