---
title: Utilize o TeamViewer para administrar remotamente dispositivos Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1284"
- "6700008"
ms.openlocfilehash: 63e7f068f3c53240ad13d1679df460c97a1a94f4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555245"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a><span data-ttu-id="52dfd-102">Utilize o TeamViewer para administrar remotamente dispositivos Intune</span><span class="sxs-lookup"><span data-stu-id="52dfd-102">Use TeamViewer to remotely administer Intune devices</span></span>

<span data-ttu-id="52dfd-103">Os dispositivos geridos pelo Intune podem ser administrados remotamente utilizando [o TeamViewer](https://www.teamviewer.com/).</span><span class="sxs-lookup"><span data-stu-id="52dfd-103">Devices managed by Intune can be administered remotely by using [TeamViewer](https://www.teamviewer.com/).</span></span>

<span data-ttu-id="52dfd-104">Para administrar o Intune utilizando o TeamViewer, utilize estes passos:</span><span class="sxs-lookup"><span data-stu-id="52dfd-104">To administer Intune by using TeamViewer, use these steps:</span></span> 

<span data-ttu-id="52dfd-105">Comece por obter credenciais do TeamViewer para configurar o Conector TeamViewer no Intune.</span><span class="sxs-lookup"><span data-stu-id="52dfd-105">Begin by obtaining credentials from TeamViewer to set up the TeamViewer Connector on Intune.</span></span> <span data-ttu-id="52dfd-106">Isto permite que o administrador introduza credenciais no UI do Conector TeamViewer em Dispositivos, uma operação única para estabelecer a ligação entre o Intune e o serviço TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="52dfd-106">This allows the admin to enter credentials in the TeamViewer Connector UI under Devices, a one-time operation to establish the link between Intune and the TeamViewer service.</span></span>

<span data-ttu-id="52dfd-107">**Parte 1: Iniciar uma sessão com um dispositivo remoto**</span><span class="sxs-lookup"><span data-stu-id="52dfd-107">**Part 1: Start a session with a remote device**</span></span>

1. <span data-ttu-id="52dfd-108">Em **Todos os dispositivos,** selecione o dispositivo com o quais pretende iniciar uma sessão remota.</span><span class="sxs-lookup"><span data-stu-id="52dfd-108">Under **All devices**, select the device you want to start a remote session with.</span></span>
2. <span data-ttu-id="52dfd-109">De **... Mais**, selecione **Nova sessão de assistência remota**.</span><span class="sxs-lookup"><span data-stu-id="52dfd-109">From  **…More**, select **New remote assistance session**.</span></span>
3. <span data-ttu-id="52dfd-110">Selecione **Sim** para reconhecer que deseja estabelecer uma sessão remota.</span><span class="sxs-lookup"><span data-stu-id="52dfd-110">Select **Yes** to acknowledge you want to establish a remote session.</span></span>
    <span data-ttu-id="52dfd-111">Depois de o pedido de "Iniciar uma nova sessão remota" ser reconhecido pelo serviço TeamViewer, verá uma opção para Iniciar assistência **remota** sob os detalhes do painel Desíduo (ou, Essencial) para o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="52dfd-111">After the "Initiating a new remote session" request is acknowledged by the TeamViewer service, you'll see an option to **Start remote assistance** under the details of the Overview (or, Essentials) pane for the device.</span></span> <span data-ttu-id="52dfd-112">Selecione **Ver Mais** para expandir o painel e mostrar o estado de Assistência Remota.</span><span class="sxs-lookup"><span data-stu-id="52dfd-112">Select **See More** to expand the pane and show the Remote Assistance status.</span></span>
4. <span data-ttu-id="52dfd-113">Selecione **Iniciar sessão remota** para iniciar a sessão no lado da administração.</span><span class="sxs-lookup"><span data-stu-id="52dfd-113">Select **Start remote session** to initiate the session on the admin side.</span></span>
5. <span data-ttu-id="52dfd-114">Opte por descarregar o binário TeamViewer (Windows) e selecione **Executar**.</span><span class="sxs-lookup"><span data-stu-id="52dfd-114">Choose to download the TeamViewer binary (Windows), and select **Run**.</span></span><br/>
    <span data-ttu-id="52dfd-115">**Nota** Pode ignorar qualquer página de navegador aberta no web site do TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="52dfd-115">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

6. <span data-ttu-id="52dfd-116">Reconheça o pedido da aplicação TeamViewer para escamar alterações no dispositivo (apenas windows).</span><span class="sxs-lookup"><span data-stu-id="52dfd-116">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
7. <span data-ttu-id="52dfd-117">A aplicação TeamViewer começa e inclui o código de sessão para autenticar a ligação com o dispositivo remoto.</span><span class="sxs-lookup"><span data-stu-id="52dfd-117">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>

<span data-ttu-id="52dfd-118">**Parte 2: No dispositivo que está a ser alvo de uma sessão remota**</span><span class="sxs-lookup"><span data-stu-id="52dfd-118">**Part 2: On the device being targeted for a remote session**</span></span>

1. <span data-ttu-id="52dfd-119">Abra o portal da empresa Intune.</span><span class="sxs-lookup"><span data-stu-id="52dfd-119">Open the Intune company portal.</span></span>
2. <span data-ttu-id="52dfd-120">Procure uma bandeira de notificação: "O seu administrador de TI está a solicitar o controlo deste dispositivo para uma sessão de assistência remota", e selecione a notificação.</span><span class="sxs-lookup"><span data-stu-id="52dfd-120">Look for a notification flag: "Your IT administrator is requesting control of this device for a remote assistance session," and select the notification.</span></span>
3. <span data-ttu-id="52dfd-121">Opte por descarregar a aplicação TeamViewer ou reconheça o download da aplicação TeamViewer a partir da loja de aplicações e selecione **Run**.</span><span class="sxs-lookup"><span data-stu-id="52dfd-121">Choose to download the TeamViewer application, or acknowledge download of the TeamViewer app from the app store, and select **Run**.</span></span>
    <span data-ttu-id="52dfd-122">**Nota** Pode ignorar qualquer página de navegador aberta no web site do TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="52dfd-122">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

4. <span data-ttu-id="52dfd-123">Reconheça o pedido da aplicação TeamViewer para escamar alterações no dispositivo (apenas windows).</span><span class="sxs-lookup"><span data-stu-id="52dfd-123">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
5. <span data-ttu-id="52dfd-124">A aplicação TeamViewer começa e inclui o código de sessão para autenticar a ligação com o dispositivo remoto.</span><span class="sxs-lookup"><span data-stu-id="52dfd-124">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>
6. <span data-ttu-id="52dfd-125">Um pop-up pergunta se quer permitir que a sessão comece.</span><span class="sxs-lookup"><span data-stu-id="52dfd-125">A popup asks if you want to allow the session to start.</span></span>

<span data-ttu-id="52dfd-126">**Nota** Os códigos de sessão gerados pelo serviço TeamViewer são utilizados apenas uma vez.</span><span class="sxs-lookup"><span data-stu-id="52dfd-126">**Note** The session codes generated by the TeamViewer service are one-time use only.</span></span> <span data-ttu-id="52dfd-127">Se perder a ligação, deve:</span><span class="sxs-lookup"><span data-stu-id="52dfd-127">If you lose the connection, you must:</span></span>

1. <span data-ttu-id="52dfd-128">Feche a instância da aplicação TeamViewer no dispositivo remoto e na estação de trabalho de administração.</span><span class="sxs-lookup"><span data-stu-id="52dfd-128">Close the instance of the TeamViewer app on the remote device and on the admin workstation.</span></span>
2. <span data-ttu-id="52dfd-129">Feche o portal da empresa no dispositivo remoto.</span><span class="sxs-lookup"><span data-stu-id="52dfd-129">Close the company portal on the remote device.</span></span>
3. <span data-ttu-id="52dfd-130">Inicie uma nova "nova sessão de assistência remota" a partir do portal de administração.</span><span class="sxs-lookup"><span data-stu-id="52dfd-130">Initiate a new "New remote Assistance session" from the admin portal.</span></span>
4. <span data-ttu-id="52dfd-131">Reabrimos o portal da empresa no dispositivo remoto para receber a nova notificação.</span><span class="sxs-lookup"><span data-stu-id="52dfd-131">Re-open the company portal on the remote device to receive the new notification.</span></span>
5. <span data-ttu-id="52dfd-132">Descarregue e abra a aplicação TeamViewer tanto no dispositivo remoto como na estação de trabalho de administração, como antes.</span><span class="sxs-lookup"><span data-stu-id="52dfd-132">Download and open the TeamViewer app on both the remote device and the admin workstation, as before.</span></span>