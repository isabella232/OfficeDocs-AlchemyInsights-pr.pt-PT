---
title: Problemas de resolução de problemas usando Open with Explorer
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: e7fe59b94d216d89c2f2f7100a3d8bf7a0b0196e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659069"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="6053e-102">Corrigir problemas com Abrir com Explorador</span><span class="sxs-lookup"><span data-stu-id="6053e-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="6053e-103">Corrija problemas comuns com a abertura de uma biblioteca de documentos no SharePoint ou No OneDrive utilizando o comando **Open with Explorer:**</span><span class="sxs-lookup"><span data-stu-id="6053e-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="6053e-104">Utilize o Internet Explorer 10 ou o Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="6053e-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="6053e-105">**Abrir com o Explorer** não é compatível com o Microsoft Edge, Google Chrome, Firefox e outros.</span><span class="sxs-lookup"><span data-stu-id="6053e-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="6053e-106">**Aberto com o Explorer** é desativado em todos os navegadores, exceto no Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="6053e-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="6053e-107">**Open with Explorer** não está disponível na experiência moderna para bibliotecas SharePoint.</span><span class="sxs-lookup"><span data-stu-id="6053e-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="6053e-108">Use **a vista no Explorador de Ficheiros** em vez disso.</span><span class="sxs-lookup"><span data-stu-id="6053e-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="6053e-109">Selecione **Ver opções** \> **Ver no Explorador de Ficheiros**.</span><span class="sxs-lookup"><span data-stu-id="6053e-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="6053e-110">A visualização no File Explorer não é compatível com o Microsoft Edge, Google Chrome, Firefox e outros.</span><span class="sxs-lookup"><span data-stu-id="6053e-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="6053e-111">**Ver no File Explorer** disponível apenas no Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="6053e-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="6053e-112">Certifique-se de que o serviço WebClient está em funcionamento.</span><span class="sxs-lookup"><span data-stu-id="6053e-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="6053e-113">Na caixa de pesquisa do Windows, escreva, selecione a aplicação de ambiente de trabalho Run, escreva serviços.msc e, em seguida, prima Enter.</span><span class="sxs-lookup"><span data-stu-id="6053e-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="6053e-114">Desloque-se até ao serviço WebClient e certifique-se de que a coluna **Status** apresenta "Running".</span><span class="sxs-lookup"><span data-stu-id="6053e-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="6053e-115">Se não o fizer, clique duas vezes no serviço, clique em **Iniciar**e, em seguida, clique **em OK**.</span><span class="sxs-lookup"><span data-stu-id="6053e-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="6053e-116">(Pode ser necessário ativar primeiro o serviço selecionando **manual** ou **automático** na caixa **tipo Arranque.)**</span><span class="sxs-lookup"><span data-stu-id="6053e-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="6053e-117">Abrir uma biblioteca no File Explorer é útil se precisar copiar ou mover vários ficheiros e pastas uma vez, mas se quiser trabalhar regularmente na biblioteca, recomendamos que o sincronize.</span><span class="sxs-lookup"><span data-stu-id="6053e-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="6053e-118">Para resolver problemas de abertura no Explorador de Ficheiros, consulte [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="6053e-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="6053e-119">Para obter informações sobre a configuração da sincronização, consulte [os ficheiros Sync SharePoint com o novo cliente de sincronização OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="6053e-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="6053e-120">Consulte o artigo [Como utilizar o comando "Abrir com explorador" para resolver problemas no SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="6053e-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

