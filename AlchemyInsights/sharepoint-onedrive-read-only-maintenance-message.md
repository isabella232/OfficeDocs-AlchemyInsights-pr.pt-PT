---
title: Read-Only para mensagem de manutenção ao tentar utilizar SharePoint ou OneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: a3d313816beefcefa4d93528d3ad9a684e60390e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670843"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="56361-102">Read-Only para mensagem de manutenção ao tentar utilizar SharePoint ou OneDrive</span><span class="sxs-lookup"><span data-stu-id="56361-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="56361-103">Os utilizadores podem receber uma mensagem **Read-Only para Manutenção** quando tentarem utilizar o SharePoint ou o OneDrive para um dos seguintes cenários.</span><span class="sxs-lookup"><span data-stu-id="56361-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="56361-104">Uma atividade de manutenção planeada ou ativa.</span><span class="sxs-lookup"><span data-stu-id="56361-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="56361-105">Verifique-os navegando no [Centro de Mensagens.](https://portal.office.com/adminportal/home#/messagecenter)</span><span class="sxs-lookup"><span data-stu-id="56361-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="56361-106">Um incidente de serviço ativo de alta prioridade que pode estar a ocorrer.</span><span class="sxs-lookup"><span data-stu-id="56361-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="56361-107">Verifique se há avisos/incidentes navegando para a [Saúde do Serviço](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="56361-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="56361-108">Um pequeno cenário de recuperação automática que pode estar a acontecer devido a eventos inesperados nos servidores que podem durar menos de 30 min ou mais.</span><span class="sxs-lookup"><span data-stu-id="56361-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="56361-109">Não existem postos de Mensagem ou Serviços de Saúde para estas pequenas recuperações, mas deverá voltar ao normal muito em breve.</span><span class="sxs-lookup"><span data-stu-id="56361-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="56361-110">Em poucas ocasiões, observámos que um dos três cenários listados acima foram a causa, e o serviço foi restaurado, mas a cache do navegador dos utilizadores não foi limpa.</span><span class="sxs-lookup"><span data-stu-id="56361-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="56361-111">Por favor, tente limpar a cache do navegador antes de navegar para o site.</span><span class="sxs-lookup"><span data-stu-id="56361-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="56361-112">No seu navegador Microsoft Edge, selecione **Definições**e, em seguida, selecione **Privacidade e Segurança**.</span><span class="sxs-lookup"><span data-stu-id="56361-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="56361-113">Em **Navegação Clara,** **selecione Escolha o que limpar**.</span><span class="sxs-lookup"><span data-stu-id="56361-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="56361-114">Selecione **Cookies e guarde os dados do site,** e selecione **Clear**.</span><span class="sxs-lookup"><span data-stu-id="56361-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="56361-115">Estes passos podem diferir quando se utilizam outros navegadores como o Mozilla Firefox ou o Google Chrome.</span><span class="sxs-lookup"><span data-stu-id="56361-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="56361-116">Outra opção seria abrir o seu site SharePoint ou OneDrive numa nova janela InPrivate.</span><span class="sxs-lookup"><span data-stu-id="56361-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>