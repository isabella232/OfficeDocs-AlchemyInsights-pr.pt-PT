---
title: Abrir com o Explorer não funciona
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 5bf28982533d8ca9998605cf3592f317c0ef99b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47694467"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="13429-102">Abrir com o Explorer não está a funcionar</span><span class="sxs-lookup"><span data-stu-id="13429-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="13429-103">Se **abrir com o Explorer** ou a View in File **Explorer** não funcionar, certifique-se de que o serviço WebClient está definido para **executar** seguindo os passos abaixo.</span><span class="sxs-lookup"><span data-stu-id="13429-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="13429-104">Por exemplo, pode levar muito tempo a abrir uma biblioteca SharePoint ou OneDrive quando o serviço não está a funcionar.</span><span class="sxs-lookup"><span data-stu-id="13429-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="13429-105">Na caixa de pesquisa do Windows, escreva, selecione a aplicação de ambiente de trabalho Run, escreva serviços.msc e, em seguida, selecione **Enter**.</span><span class="sxs-lookup"><span data-stu-id="13429-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="13429-106">Percorra o serviço WebClient e verifique a coluna **Status.**</span><span class="sxs-lookup"><span data-stu-id="13429-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="13429-107">Se o estado de serviço webClient não estiver **a funcionar,** clique duas vezes no serviço, clique em **Iniciar**e, em seguida, clique **em OK**.</span><span class="sxs-lookup"><span data-stu-id="13429-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="13429-108">Ativar o serviço, se necessário, selecionando **manual** ou **automático** na caixa **do tipo Arranque.**</span><span class="sxs-lookup"><span data-stu-id="13429-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="13429-109">Para resolver problemas de abertura no Explorador de Ficheiros, consulte [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="13429-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="13429-110">Explore a sincronização como uma alternativa melhor: [Sync SharePoint com o novo cliente de sincronização OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="13429-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

