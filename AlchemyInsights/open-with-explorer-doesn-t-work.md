---
title: Abrir com o Explorador não funciona
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 7680766b53bd5e85789375d3f9e9ab635780ec6c
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36538494"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="c5634-102">Abrir com o Explorer não está a funcionar</span><span class="sxs-lookup"><span data-stu-id="c5634-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="c5634-103">Se **Abrir com o Explorador** ou **vista do Explorador de ficheiros** não funciona certificar-se de que o serviço WebClient está definido para **ser executado** , seguindo os passos abaixo.</span><span class="sxs-lookup"><span data-stu-id="c5634-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="c5634-104">Por exemplo, poderá demorar muito tempo a abrir uma biblioteca de SharePoint ou OneDrive quando o serviço não está em execução.</span><span class="sxs-lookup"><span data-stu-id="c5634-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="c5634-105">Na caixa de procura do Windows, o tipo de executar, seleccione a executar aplicações de ambiente de trabalho, tipo msc e, em seguida, seleccione **Enter**.</span><span class="sxs-lookup"><span data-stu-id="c5634-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="c5634-106">Desloque-se para o serviço WebClient e verificar a coluna de **Estado** .</span><span class="sxs-lookup"><span data-stu-id="c5634-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="c5634-107">Se o estado do serviço WebClient não está **em execução**, faça duplo clique sobre o serviço, clique em **Iniciar**e, em seguida, clique em **OK**.</span><span class="sxs-lookup"><span data-stu-id="c5634-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="c5634-108">Active o serviço, se necessário, seleccionando o **Manual** ou **Automático** na caixa **tipo de arranque** .</span><span class="sxs-lookup"><span data-stu-id="c5634-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="c5634-109">Para resolver problemas de abertura no Explorador de ficheiros, consulte [aberta no Explorador](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="c5634-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="c5634-110">Explorar sincronização como uma melhor alternativa: [ficheiros do SharePoint de sincronização com o novo cliente de sincronização de OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="c5634-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

