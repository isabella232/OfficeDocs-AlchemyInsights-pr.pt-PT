---
title: Aberto com Explorer não funciona
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: dc939a3451ff4fe95e4aa5a999839a2c532b398c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713045"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="89edb-102">Abrir com explorador não está funcionando</span><span class="sxs-lookup"><span data-stu-id="89edb-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="89edb-103">Se **abrir com o Explorer** ou ver no File **Explorer** não funcionar, certifique-se de que o serviço WebClient está definido para **Executar** seguindo os passos abaixo.</span><span class="sxs-lookup"><span data-stu-id="89edb-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="89edb-104">Por exemplo, pode levar muito tempo para abrir uma biblioteca SharePoint ou OneDrive quando o serviço não estiver em execução.</span><span class="sxs-lookup"><span data-stu-id="89edb-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="89edb-105">Na caixa de pesquisa do Windows, digite, selecione a aplicação de ambiente de trabalho Run, escreva serviços.msc e, em seguida, selecione **Enter**.</span><span class="sxs-lookup"><span data-stu-id="89edb-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="89edb-106">Desloque-se até ao serviço WebClient e verifique a coluna **'Status'.**</span><span class="sxs-lookup"><span data-stu-id="89edb-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="89edb-107">Se o estado de serviço do WebClient não estiver **a funcionar,** clique duas vezes no serviço, clique em **Iniciar**, e clique em **OK**.</span><span class="sxs-lookup"><span data-stu-id="89edb-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="89edb-108">Ativar o serviço, se necessário, selecionando **manual** ou **automático** na caixa **do tipo Arranque.**</span><span class="sxs-lookup"><span data-stu-id="89edb-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="89edb-109">Para resolver problemas de abertura no File Explorer, consulte [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="89edb-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="89edb-110">Explore a sincronização como uma alternativa melhor: [Sync SharePoint ficheiros com o novo cliente sincronizado OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="89edb-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

