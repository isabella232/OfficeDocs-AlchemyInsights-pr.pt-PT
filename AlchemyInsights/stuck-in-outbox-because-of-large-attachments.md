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
ms.openlocfilehash: 4f69de167dc51961fa7cf71b4d73ca7ee3ed4d55
ms.sourcegitcommit: 57fb994ddd3854d06faa67680c971b003b06bf83
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/13/2020
ms.locfileid: "43241263"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="ea7d8-102">Corrija mensagens que estão presas na Caixa de Saída</span><span class="sxs-lookup"><span data-stu-id="ea7d8-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="ea7d8-103">Recomendamos que comece por executar o cenário ["Estou com problemas em enviar, receber ou encontrar mensagens](https://aka.ms/SaRA-OutlookSendReceive) de correio eletrónico" da ferramenta [Microsoft Support and Recovery Assistant.](https://diagnostics.office.com/#/)</span><span class="sxs-lookup"><span data-stu-id="ea7d8-103">We recommend that you start by running the scenario ["I'm having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool.</span></span>

<span data-ttu-id="ea7d8-104">Quando uma mensagem fica presa na sua Outbox, a causa mais provável é um grande anexo ou a opção "Enviar imediatamente quando estiver ligada" não está ativada.</span><span class="sxs-lookup"><span data-stu-id="ea7d8-104">When a message gets stuck in your Outbox, the most likely cause is a large attachment or the option "Send immediately when connected" is not enabled.</span></span>

<span data-ttu-id="ea7d8-105">**Retire o acessório grande**</span><span class="sxs-lookup"><span data-stu-id="ea7d8-105">**Remove the large attachment**</span></span>

1. <span data-ttu-id="ea7d8-106">No Outlook, selecione **Enviar / Receber** > **Trabalho Offline**.</span><span class="sxs-lookup"><span data-stu-id="ea7d8-106">In Outlook, select **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="ea7d8-107">No painel de navegação, selecione **Outbox**.</span><span class="sxs-lookup"><span data-stu-id="ea7d8-107">In the navigation pane, select **Outbox**.</span></span> <span data-ttu-id="ea7d8-108">A partir daqui, pode:</span><span class="sxs-lookup"><span data-stu-id="ea7d8-108">From here, you can:</span></span> 
    - <span data-ttu-id="ea7d8-109">Apagar a mensagem (selecione-a e, em seguida, **selecione Apagar**).</span><span class="sxs-lookup"><span data-stu-id="ea7d8-109">Delete the message (select it and then select **Delete**).</span></span>
    - <span data-ttu-id="ea7d8-110">Arraste a mensagem para a pasta Drafts, clique duas vezes para abri-la e remova o anexo selecione-o e, em seguida, **selecione Delete**).</span><span class="sxs-lookup"><span data-stu-id="ea7d8-110">Drag the message to your Drafts folder, double-click to open it, and remove the attachment select it and then select **Delete**).</span></span>
3. <span data-ttu-id="ea7d8-111">Se receber um erro que diga que o Outlook está a tentar transmitir a mensagem, feche o Outlook.</span><span class="sxs-lookup"><span data-stu-id="ea7d8-111">If you receive an error that says Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="ea7d8-112">Pode levar alguns momentos para sair.</span><span class="sxs-lookup"><span data-stu-id="ea7d8-112">It may take a few moments to exit.</span></span> <span data-ttu-id="ea7d8-113">Se o Outlook não fechar, prima Ctrl+Alt+Delete e selecione **Start Task Manager**.</span><span class="sxs-lookup"><span data-stu-id="ea7d8-113">If Outlook doesn't close, press Ctrl+Alt+Delete and select **Start Task Manager**.</span></span> <span data-ttu-id="ea7d8-114">No Gestor de Tarefas, selecione o separador **Processos,** desloque-se para outlook.exe e selecione **End Process**.</span><span class="sxs-lookup"><span data-stu-id="ea7d8-114">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and select **End Process**.</span></span>
4. <span data-ttu-id="ea7d8-115">Depois do Outlook fechar, reinicie-o e repita os passos 2 e 3.</span><span class="sxs-lookup"><span data-stu-id="ea7d8-115">After Outlook closes, restart it and repeat steps 2 and 3.</span></span> 
5. <span data-ttu-id="ea7d8-116">Depois de remover o anexo, clique em **Enviar / Receber** > **Trabalho Offline** para retomar o trabalho online.</span><span class="sxs-lookup"><span data-stu-id="ea7d8-116">After you remove the attachment, click **Send / Receive** > **Work Offline** to resume working online.</span></span> 

<span data-ttu-id="ea7d8-117">As mensagens também ficam presas na Caixa de Saída quando clica em **Enviar**, mas não está ligada.</span><span class="sxs-lookup"><span data-stu-id="ea7d8-117">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="ea7d8-118">Clique em **Enviar / Receber** e ver o botão Work **Offline.**</span><span class="sxs-lookup"><span data-stu-id="ea7d8-118">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="ea7d8-119">Se é azul, estás desligado.</span><span class="sxs-lookup"><span data-stu-id="ea7d8-119">If it's blue, you're disconnected.</span></span> <span data-ttu-id="ea7d8-120">Clique nele para ligar (o botão fica branco) e clique em **Enviar tudo**.</span><span class="sxs-lookup"><span data-stu-id="ea7d8-120">Click it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="ea7d8-121">**Ativar Enviar imediatamente quando ligado**</span><span class="sxs-lookup"><span data-stu-id="ea7d8-121">**Enable Send immediately when connected**</span></span>
 
1. <span data-ttu-id="ea7d8-122">No separador Ficheiro, clique em **Opções**.</span><span class="sxs-lookup"><span data-stu-id="ea7d8-122">On the File tab, click **Options**.</span></span>

2. <span data-ttu-id="ea7d8-123">Na caixa de diálogo Outlook Options, clique **em Advanced**.</span><span class="sxs-lookup"><span data-stu-id="ea7d8-123">In the Outlook Options dialog box, click **Advanced**.</span></span>

3. <span data-ttu-id="ea7d8-124">Na secção Enviar e receber, clique para ativar **Enviar imediatamente quando ligado**.</span><span class="sxs-lookup"><span data-stu-id="ea7d8-124">In the Send and receive section, click to enable **Send immediately when connected**.</span></span> <span data-ttu-id="ea7d8-125">Clique em **OK**.</span><span class="sxs-lookup"><span data-stu-id="ea7d8-125">Click **OK**.</span></span>
 
<span data-ttu-id="ea7d8-126">Para mais detalhes, consulte:</span><span class="sxs-lookup"><span data-stu-id="ea7d8-126">For full details, see:</span></span>
- [<span data-ttu-id="ea7d8-127">Vídeo: Enviar ou apagar um e-mail preso</span><span class="sxs-lookup"><span data-stu-id="ea7d8-127">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="ea7d8-128">O e-mail permanece na pasta Outbox até iniciar manualmente uma operação de envio/receção no Outlook</span><span class="sxs-lookup"><span data-stu-id="ea7d8-128">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
