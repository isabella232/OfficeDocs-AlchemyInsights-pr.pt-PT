---
title: Ativar Teams Webinars
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11513"
- "9006672"
ms.openlocfilehash: 5a732e6746e9fd23e54a0b2ffeabb59623012a0e
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/04/2021
ms.locfileid: "52793782"
---
# <a name="enable-teams-webinars"></a><span data-ttu-id="95253-102">Ativar Teams Webinars</span><span class="sxs-lookup"><span data-stu-id="95253-102">Enable Teams Webinars</span></span>

<span data-ttu-id="95253-103">Os webinars estão ativados por predefinição.</span><span class="sxs-lookup"><span data-stu-id="95253-103">Webinars are enabled by default.</span></span> <span data-ttu-id="95253-104">Pode gerir quem pode agendar e registar-se em Webinars Teams utilizando Teams comandos do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="95253-104">You can manage who can schedule and register for Teams Webinars by using Teams PowerShell commands.</span></span>

- <span data-ttu-id="95253-105">Todos os utilizadores que podem criar uma reunião também podem criar uma reunião de webinar.</span><span class="sxs-lookup"><span data-stu-id="95253-105">All users who can create a meeting can also create a webinar meeting.</span></span> <span data-ttu-id="95253-106">Se quiser gerir quem pode agendar Webinars Teams, utilize *AllowMeetingRegistration.*</span><span class="sxs-lookup"><span data-stu-id="95253-106">If you want to manage who can schedule Teams Webinars, use *AllowMeetingRegistration*.</span></span> 
- <span data-ttu-id="95253-107">Por *predefinição, o WhoCanRegister* está ativado e definido como **Todos.**</span><span class="sxs-lookup"><span data-stu-id="95253-107">By default, *WhoCanRegister* is enabled and set to **Everyone**.</span></span> <span data-ttu-id="95253-108">Se quiser destivar o registo de reuniões, *defina AllowMeetingRegistration* como **Falso.**</span><span class="sxs-lookup"><span data-stu-id="95253-108">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="95253-109">Para alterar estas definições, tem de instalar o [Teams PowerShell.](/microsoftteams/teams-powershell-install)</span><span class="sxs-lookup"><span data-stu-id="95253-109">To change these settings, you must install [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> <span data-ttu-id="95253-110">Além disso, as Políticas de Reunião são impodas Teams webinars.</span><span class="sxs-lookup"><span data-stu-id="95253-110">Also, Meeting Policies are enforced on Teams Webinars.</span></span> <span data-ttu-id="95253-111">Por exemplo, se a associação anónima estiver desligada nas definições da reunião, os utilizadores anónimos não podem participar em webinars.</span><span class="sxs-lookup"><span data-stu-id="95253-111">For example, if anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span>

<span data-ttu-id="95253-112">Para saber mais sobre como configurar quem pode registar-se em webinars, consulte Configurar quem pode registar-se [em webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span><span class="sxs-lookup"><span data-stu-id="95253-112">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="95253-113">Para obter mais informações sobre as definições das Listas Microsoft, consulte [Definições de controlo para o Microsoft Lists.](/sharepoint/control-lists)</span><span class="sxs-lookup"><span data-stu-id="95253-113">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>