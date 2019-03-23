---
title: Resolver problemas utilizando abrir com o Explorer
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: 03bb3ad01a716390ec50845b29ddf6cc81a83116
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/22/2019
ms.locfileid: "30759305"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="e84df-102">Corrigir problemas com aberto com o Explorer</span><span class="sxs-lookup"><span data-stu-id="e84df-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="e84df-103">Corrigir problemas comuns com a abertura de uma biblioteca de documentos no SharePoint ou utilizando o comando **Abrir com o Explorador** de OneDrive:</span><span class="sxs-lookup"><span data-stu-id="e84df-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="e84df-104">Utilizar o Internet Explorer 10 ou 11 do Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="e84df-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="e84df-105">**Abrir com o Explorador** não é compatível com Microsoft Edge, Google Chrome, Firefox e outros utilizadores.</span><span class="sxs-lookup"><span data-stu-id="e84df-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="e84df-106">**Abrir com o Explorador** está desactivada em todos os browsers, excepto o Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="e84df-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="e84df-107">**Abrir com o Explorador** não está disponível na experiência moderna de bibliotecas do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="e84df-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="e84df-108">Utilize a **vista do Explorador de ficheiros** .</span><span class="sxs-lookup"><span data-stu-id="e84df-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="e84df-109">Seleccione **Opções de visualização** \> **vista do Explorador de ficheiros**.</span><span class="sxs-lookup"><span data-stu-id="e84df-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="e84df-110">Vista do Explorador de ficheiros não é compatível com Microsoft Edge, Google Chrome, Firefox e outros utilizadores.</span><span class="sxs-lookup"><span data-stu-id="e84df-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="e84df-111">**Vista do Explorador de ficheiros** disponíveis apenas no Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="e84df-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="e84df-112">Certifique-se do que serviço WebClient está em execução.</span><span class="sxs-lookup"><span data-stu-id="e84df-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="e84df-113">Na caixa de pesquisa do Windows, introduza executar, seleccione a aplicação de ambiente de trabalho de execução, escreva Services. msc e, em seguida, prima Enter.</span><span class="sxs-lookup"><span data-stu-id="e84df-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="e84df-114">Desloque-se para o serviço WebClient e certificar-se de que a coluna de **Estado** apresenta "Executar".</span><span class="sxs-lookup"><span data-stu-id="e84df-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="e84df-115">Caso contrário, faça duplo clique sobre o serviço, clique em **Iniciar**e, em seguida, clique em **OK**.</span><span class="sxs-lookup"><span data-stu-id="e84df-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="e84df-116">(Poderá ter de activar primeiro o serviço seleccionando **Manual** ou **Automático** na caixa **tipo de arranque** .)</span><span class="sxs-lookup"><span data-stu-id="e84df-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="e84df-117">Abrir uma biblioteca no Explorador de ficheiros é útil se necessitar de copiar ou mover vários ficheiros e pastas, uma vez, mas se pretender trabalhar regularmente na biblioteca, recomendamos sincronizar.</span><span class="sxs-lookup"><span data-stu-id="e84df-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="e84df-118">Para resolver problemas de abertura no Explorador de ficheiros, consulte [aberta no Explorador](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="e84df-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="e84df-119">Para informações sobre como configurar a sincronização, consulte [ficheiros de sincronização SharePoint com o novo cliente de sincronização de OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="e84df-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="e84df-120">Consulte o artigo [como utilizar o comando ' Abrir com o Explorer ' para resolver problemas no SharePoint Online](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="e84df-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) for more information.</span></span> 
  

