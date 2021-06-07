---
title: Gerir o registo de webinars
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
- "11512"
- "9006672"
ms.openlocfilehash: c5b0721d286b07d7e0f84199885b6f527a2b42a2
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793911"
---
# <a name="manage-webinar-registration"></a><span data-ttu-id="aadcd-102">Gerir o registo de webinars</span><span class="sxs-lookup"><span data-stu-id="aadcd-102">Manage webinar registration</span></span>

<span data-ttu-id="aadcd-103">Pode gerir quem pode registar-se Teams Webinars ao utilizar Teams comandos do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="aadcd-103">You manage who can register for Teams Webinars by using Teams Powershell commands.</span></span> <span data-ttu-id="aadcd-104">Para instalar Teams PowerShell, consulte o [Teams PowerShell.](/microsoftteams/teams-powershell-install)</span><span class="sxs-lookup"><span data-stu-id="aadcd-104">To install Teams Powershell, see [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> 

<span data-ttu-id="aadcd-105">Por *predefinição, o WhoCanRegister* está ativado e definido para **EveryoneInCompany.**</span><span class="sxs-lookup"><span data-stu-id="aadcd-105">By default, *WhoCanRegister* is enabled and set to **EveryoneInCompany**.</span></span> <span data-ttu-id="aadcd-106">Para permitir que qualquer pessoa, incluindo utilizadores anónimos, se registe, tem de definir a Política de Reunião para Todos utilizando o comando do PowerShell: </span><span class="sxs-lookup"><span data-stu-id="aadcd-106">To allow anyone, including anonymous users, to register, you must set the Meeting Policy to **Everyone** by using the Powershell command:</span></span>

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

<span data-ttu-id="aadcd-107">**Nota:** se a associação anónima estiver desligada nas definições da reunião, os utilizadores anónimos não podem participar em webinars.</span><span class="sxs-lookup"><span data-stu-id="aadcd-107">**Note**: If anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span> <span data-ttu-id="aadcd-108">Para saber mais e ativar esta definição, consulte [Gerir definições de reunião no Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span><span class="sxs-lookup"><span data-stu-id="aadcd-108">To learn more and enable this setting, see [Manage meeting settings in Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span></span>

<span data-ttu-id="aadcd-109">Se quiser destivar o registo de reuniões, *defina AllowMeetingRegistration* como **Falso.**</span><span class="sxs-lookup"><span data-stu-id="aadcd-109">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="aadcd-110">Para saber mais sobre como configurar quem pode registar-se em webinars, consulte Configurar quem pode registar-se [em webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span><span class="sxs-lookup"><span data-stu-id="aadcd-110">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="aadcd-111">Para obter mais informações sobre as definições das Listas Microsoft, consulte [Definições de controlo para o Microsoft Lists.](/sharepoint/control-lists)</span><span class="sxs-lookup"><span data-stu-id="aadcd-111">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>
