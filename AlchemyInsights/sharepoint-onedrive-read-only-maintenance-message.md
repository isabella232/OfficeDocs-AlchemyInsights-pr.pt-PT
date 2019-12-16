---
title: Leia-somente para a mensagem de manutenção ao tentar usar sharepoint ou onedrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 02cf1aa7abae365a3d317af9e785648d1c1517e1
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051292"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="97396-102">Leia-somente para a mensagem de manutenção ao tentar usar sharepoint ou onedrive</span><span class="sxs-lookup"><span data-stu-id="97396-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="97396-103">Os usuários podem receber uma mensagem **de leitura somente para manutenção** ao tentar usar o SharePoint ou o OneDrive para um dos seguintes cenários.</span><span class="sxs-lookup"><span data-stu-id="97396-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="97396-104">Uma atividade de manutenção planejada ou ativa.</span><span class="sxs-lookup"><span data-stu-id="97396-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="97396-105">Verifique se eles, navegando para o Centro de [Mensagens](https://portal.office.com/adminportal/home#/messagecenter).</span><span class="sxs-lookup"><span data-stu-id="97396-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="97396-106">Um incidente de serviço ativo de alta prioridade que pode estar ocorrendo.</span><span class="sxs-lookup"><span data-stu-id="97396-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="97396-107">Verifique se há avisos/incidentes navegando para o [Serviço de Saúde.](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="97396-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="97396-108">Um cenário de recuperação de auto-cura menor que poderia estar acontecendo devido a quaisquer eventos inesperados nos servidores que podem durar menos de 30 min ou assim.</span><span class="sxs-lookup"><span data-stu-id="97396-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="97396-109">Não há mensagens do Centro de Mensagens ou de Saúde de Serviço para essas pequenas recuperações, mas você deve estar de volta ao normal muito em breve.</span><span class="sxs-lookup"><span data-stu-id="97396-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="97396-110">Em poucas ocasiões, observamos que um dos três cenários listados acima foi a causa, e o serviço foi restaurado, mas o cache do navegador de usuários não foi esclarecido.</span><span class="sxs-lookup"><span data-stu-id="97396-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="97396-111">Por favor, tente limpar o cache do navegador antes de navegar para o site.</span><span class="sxs-lookup"><span data-stu-id="97396-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="97396-112">No navegador Microsoft Edge, selecione **configurações**e selecione **privacidade e segurança.**</span><span class="sxs-lookup"><span data-stu-id="97396-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="97396-113">Em **navegação clara,** **selecione escolha o que limpar.**</span><span class="sxs-lookup"><span data-stu-id="97396-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="97396-114">Selecione **cookies e economizou dados**do site, e **selecione Clear**.</span><span class="sxs-lookup"><span data-stu-id="97396-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="97396-115">Essas etapas podem diferir ao usar outros navegadores, como o Mozilla Firefox ou o Google Chrome.</span><span class="sxs-lookup"><span data-stu-id="97396-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="97396-116">Outra opção seria abrir seu site SharePoint ou OneDrive em uma nova janela InPrivate.</span><span class="sxs-lookup"><span data-stu-id="97396-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>