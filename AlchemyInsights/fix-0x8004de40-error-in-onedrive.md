---
title: Corrigir o erro de 0x8004de40 em OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 2256fb66cb7a4e2adcff9fda16a80c87e2997f0c
ms.sourcegitcommit: 8f6a1be929b275faa295ba8aeeae17898a47c3b0
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/21/2019
ms.locfileid: "35133987"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="74d91-102">Corrigir o erro de 0x8004de40 em OneDrive</span><span class="sxs-lookup"><span data-stu-id="74d91-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="74d91-103">Se receber um erro de 0x8004de40 com OneDrive:</span><span class="sxs-lookup"><span data-stu-id="74d91-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="74d91-104">Reinicie o computador afectado enquanto estiver ligado ao domínio do directório Acitve.</span><span class="sxs-lookup"><span data-stu-id="74d91-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="74d91-105">Se reiniciar o computador não corrigir o problema, desligar e voltar a aderir o dispositivo do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="74d91-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="74d91-106">**Nota**: deve estar na rede da empresa ao efectuar estes passos.</span><span class="sxs-lookup"><span data-stu-id="74d91-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="74d91-107">Não efectue estes passos quando não conseguir estabelecer ligação com a infra-estrutura da empresa (por exemplo, quando estou em viagem).</span><span class="sxs-lookup"><span data-stu-id="74d91-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="74d91-108">Abra uma linha de comandos elevada.</span><span class="sxs-lookup"><span data-stu-id="74d91-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="74d91-109">Para abrir uma linha de comandos elevada, clique - **Iniciar**, clique em **linha de comandos**e, em seguida, clique em **Executar como administrador**.</span><span class="sxs-lookup"><span data-stu-id="74d91-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="74d91-110">Escreva *dsregcmd /leave* e prima **Enter**.</span><span class="sxs-lookup"><span data-stu-id="74d91-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="74d91-111">Quando tiver terminado, escreva *dsregcmd /join* e prima **Enter**.</span><span class="sxs-lookup"><span data-stu-id="74d91-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="74d91-112">Quando tiver terminado, feche a linha de comandos.</span><span class="sxs-lookup"><span data-stu-id="74d91-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="74d91-113">Reinicie o computador e inicie sessão em OneDrive.</span><span class="sxs-lookup"><span data-stu-id="74d91-113">Reboot the computer, and log into OneDrive.</span></span>