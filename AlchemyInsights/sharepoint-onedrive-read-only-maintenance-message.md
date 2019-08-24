---
title: Só de leitura para mensagens de manutenção ao tentar utilizar o SharePoint ou OneDrive
ms.author: efrene
author: efrene
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
ms.openlocfilehash: 5b1e56253d6deeb0f9ba2f753eff5c00ff9c51a2
ms.sourcegitcommit: cd79ecca88b2cb166f78f44ab8bc4e8136729418
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/23/2019
ms.locfileid: "36620734"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="79e47-102">Só de leitura para mensagens de manutenção ao tentar utilizar o SharePoint ou OneDrive</span><span class="sxs-lookup"><span data-stu-id="79e47-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="79e47-103">Os utilizadores poderão receber uma mensagem **Só de leitura para manutenção** , quando tenta utilizar o SharePoint ou OneDrive para um dos seguintes cenários.</span><span class="sxs-lookup"><span data-stu-id="79e47-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="79e47-104">Uma actividade de manutenção planeada ou activa.</span><span class="sxs-lookup"><span data-stu-id="79e47-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="79e47-105">Verifique os navegando para o [Centro de mensagens](https://portal.office.com/adminportal/home#/messagecenter).</span><span class="sxs-lookup"><span data-stu-id="79e47-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="79e47-106">Incidentes de serviço activo de elevada prioridade, que podem estar a ocorrer.</span><span class="sxs-lookup"><span data-stu-id="79e47-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="79e47-107">Verificar a existência de quaisquer avisos de incidentes navegando para a [Saúde do serviço](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="79e47-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="79e47-108">Um pequena reparação automática cenário de recuperação que poderia ser acontecer devido a quaisquer acontecimentos imprevistos nos servidores que podem durar menos de 30 min., mais ou menos.</span><span class="sxs-lookup"><span data-stu-id="79e47-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="79e47-109">Não existem nenhum Centro de mensagens ou serviço de saúde regista estes pequenas recuperações mas deverá ser normal muito mais rapidamente.</span><span class="sxs-lookup"><span data-stu-id="79e47-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="79e47-110">Em ocasiões muito poucos Vamos observar que um dos três cenários listados acima ter sido a causa e serviço foi restaurado, mas ainda não foram eliminada da cache do browser os utilizadores.</span><span class="sxs-lookup"><span data-stu-id="79e47-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="79e47-111">Tente limpar a cache do browser antes de navegar para o site.</span><span class="sxs-lookup"><span data-stu-id="79e47-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="79e47-112">No browser do Microsoft Edge, seleccione **Definições**e, em seguida, seleccione a **privacidade e segurança**.</span><span class="sxs-lookup"><span data-stu-id="79e47-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="79e47-113">Em **Navegação clara**, seleccione **Escolher o que para a desmarcar**.</span><span class="sxs-lookup"><span data-stu-id="79e47-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="79e47-114">Seleccione **Cookies e dados dos Web sites guardada**e, seleccione **Limpar**.</span><span class="sxs-lookup"><span data-stu-id="79e47-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="79e47-115">Estes passos podem ser diferentes quando utiliza outros browsers, tais como o Mozilla Firefox ou o Google Chrome.</span><span class="sxs-lookup"><span data-stu-id="79e47-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="79e47-116">Outra opção seria abrir o SharePoint site ou OneDrive numa nova janela InPrivate.</span><span class="sxs-lookup"><span data-stu-id="79e47-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>