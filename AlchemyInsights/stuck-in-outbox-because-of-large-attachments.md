---
title: Preso no Outbox por causa de grandes anexos
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2713"
- "9000768"
- "9002385"
- "4645"
ms.openlocfilehash: 35fe9ae76ca77faa43796b288af09be8525cb6df
ms.sourcegitcommit: 929f8accdca2b8e5be170e0fc8edd527581453d4
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/12/2020
ms.locfileid: "43232641"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="3f190-102">Corrija mensagens que estão presas na Caixa de Saída</span><span class="sxs-lookup"><span data-stu-id="3f190-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="3f190-103">Recomendamos que comece por executar o cenário ["Estou com problemas em enviar, receber ou encontrar mensagens](https://aka.ms/SaRA-OutlookSendReceive) de correio eletrónico" da ferramenta [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) na máquina afetada.</span><span class="sxs-lookup"><span data-stu-id="3f190-103">We recommend that you start by running the scenario ["I'm having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool on the affected machine.</span></span>

<span data-ttu-id="3f190-104">Quando uma mensagem fica presa na sua Outbox, a causa mais provável é um grande anexo ou a opção "Enviar imediatamente quando estiver ligada" não está ativada.</span><span class="sxs-lookup"><span data-stu-id="3f190-104">When a message gets stuck in your Outbox, the most likely cause is a large attachment or the option "Send immediately when connected" is not enabled.</span></span>

<span data-ttu-id="3f190-105">**Retire o acessório grande**</span><span class="sxs-lookup"><span data-stu-id="3f190-105">**Remove the large attachment**</span></span>

1. <span data-ttu-id="3f190-106">Clique em **Enviar / Receber** > **trabalho offline**.</span><span class="sxs-lookup"><span data-stu-id="3f190-106">Click **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="3f190-107">No painel de navegação, clique no **Outbox**.</span><span class="sxs-lookup"><span data-stu-id="3f190-107">In the navigation pane, click **Outbox**.</span></span> <span data-ttu-id="3f190-108">A partir daqui, pode:</span><span class="sxs-lookup"><span data-stu-id="3f190-108">From here, you can:</span></span> 
    - <span data-ttu-id="3f190-109">Apague a mensagem.</span><span class="sxs-lookup"><span data-stu-id="3f190-109">Delete the message.</span></span> <span data-ttu-id="3f190-110">Basta selecioná-lo e clicar **em Apagar**.</span><span class="sxs-lookup"><span data-stu-id="3f190-110">Just select it and click **Delete**.</span></span>
    - <span data-ttu-id="3f190-111">Arraste a mensagem para a pasta de **redação,** clique em dois cliques para abrir a mensagem e elimine o anexo (clique nele e clique em **Apagar**).</span><span class="sxs-lookup"><span data-stu-id="3f190-111">Drag the message to your **drafts folder**, double-click to open the message, and delete the attachment (click it and click **Delete**).</span></span>
3. <span data-ttu-id="3f190-112">Se um erro lhe disser que o Outlook está a tentar transmitir a mensagem, feche o Outlook.</span><span class="sxs-lookup"><span data-stu-id="3f190-112">If an error tells you Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="3f190-113">Pode levar alguns momentos para sair.</span><span class="sxs-lookup"><span data-stu-id="3f190-113">It may take a few moments to exit.</span></span> <span data-ttu-id="3f190-114">Se o Outlook não fechar, prima **Ctrl+Alt+Delete** e clique em **Iniciar O Gestor de Tarefas**.</span><span class="sxs-lookup"><span data-stu-id="3f190-114">If Outlook doesn't close, press **Ctrl+Alt+Delete** and click **Start Task Manager**.</span></span> <span data-ttu-id="3f190-115">No Gestor de Tarefas, selecione o separador **Processos,** desloque-se para outlook.exe e clique em **Processo final**.</span><span class="sxs-lookup"><span data-stu-id="3f190-115">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and click **End Process**.</span></span>
4. <span data-ttu-id="3f190-116">Depois do Outlook fechar, reinicie o Outlook e repita os passos 2-3.</span><span class="sxs-lookup"><span data-stu-id="3f190-116">After Outlook closes, restart Outlook and repeat steps 2-3.</span></span> 
5. <span data-ttu-id="3f190-117">Depois de remover o acessório, clique em **Enviar / Receber** > **Trabalho Offline** para desmarcar o botão e retomar o trabalho online.</span><span class="sxs-lookup"><span data-stu-id="3f190-117">After you remove the attachment, click **Send / Receive** > **Work Offline** to deselect the button and to resume working online.</span></span> 

<span data-ttu-id="3f190-118">As mensagens também ficam presas na Caixa de Saída quando clica em **Enviar**, mas não está ligada.</span><span class="sxs-lookup"><span data-stu-id="3f190-118">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="3f190-119">Clique em **Enviar / Receber** e ver o botão Work **Offline.**</span><span class="sxs-lookup"><span data-stu-id="3f190-119">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="3f190-120">Se é azul, estás desligado.</span><span class="sxs-lookup"><span data-stu-id="3f190-120">If it's blue, you're disconnected.</span></span> <span data-ttu-id="3f190-121">Clique nele para ligar (o botão fica branco) e clique em **Enviar tudo**.</span><span class="sxs-lookup"><span data-stu-id="3f190-121">Click it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="3f190-122">**Ativar Enviar imediatamente quando ligado**</span><span class="sxs-lookup"><span data-stu-id="3f190-122">**Enable Send immediately when connected**</span></span>
 
1. <span data-ttu-id="3f190-123">No separador Ficheiro, clique em **Opções**.</span><span class="sxs-lookup"><span data-stu-id="3f190-123">On the File tab, click **Options**.</span></span>

2. <span data-ttu-id="3f190-124">Na caixa de diálogo Outlook Options, clique **em Advanced**.</span><span class="sxs-lookup"><span data-stu-id="3f190-124">In the Outlook Options dialog box, click **Advanced**.</span></span>

3. <span data-ttu-id="3f190-125">Na secção Enviar e receber, clique para ativar **Enviar imediatamente quando ligado**.</span><span class="sxs-lookup"><span data-stu-id="3f190-125">In the Send and receive section, click to enable **Send immediately when connected**.</span></span> <span data-ttu-id="3f190-126">Clique em **OK**.</span><span class="sxs-lookup"><span data-stu-id="3f190-126">Click **OK**.</span></span>
 
<span data-ttu-id="3f190-127">Para mais detalhes, consulte:</span><span class="sxs-lookup"><span data-stu-id="3f190-127">For full details, see:</span></span>
- [<span data-ttu-id="3f190-128">Vídeo: Enviar ou apagar um e-mail preso</span><span class="sxs-lookup"><span data-stu-id="3f190-128">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="3f190-129">O e-mail permanece na pasta Outbox até iniciar manualmente uma operação de envio/receção no Outlook</span><span class="sxs-lookup"><span data-stu-id="3f190-129">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
