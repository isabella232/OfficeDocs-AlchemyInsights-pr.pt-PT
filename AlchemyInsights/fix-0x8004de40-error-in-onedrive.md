---
title: Corrigir erro 0x8004de40 no OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 5da4271f242597b195ef61d553fd4a2ffb313025
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716039"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="c78d9-102">Corrigir erro 0x8004de40 no OneDrive</span><span class="sxs-lookup"><span data-stu-id="c78d9-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="c78d9-103">Se receber um erro 0x8004de40 com o OneDrive:</span><span class="sxs-lookup"><span data-stu-id="c78d9-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="c78d9-104">Reinicie o computador afetado enquanto está ligado ao seu domínio de Diretório Acitve.</span><span class="sxs-lookup"><span data-stu-id="c78d9-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="c78d9-105">Se um reboot não resolver o problema, desadere e volte a juntar-se ao seu dispositivo a partir de Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c78d9-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="c78d9-106">**Nota:** Deve estar na sua rede corporativa enquanto realiza estes passos.</span><span class="sxs-lookup"><span data-stu-id="c78d9-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="c78d9-107">Não execute estes passos quando não conseguir ligar-se à sua infraestrutura corporativa (por exemplo, durante a viagem).</span><span class="sxs-lookup"><span data-stu-id="c78d9-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="c78d9-108">Abra um pedido de comando elevado.</span><span class="sxs-lookup"><span data-stu-id="c78d9-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="c78d9-109">Para abrir um pedido de comando elevado, clique em **- Iniciar**, clique à direita No Pedido de **Comando**, e, em seguida, clique em Executar **como administrador**.</span><span class="sxs-lookup"><span data-stu-id="c78d9-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="c78d9-110">Digite *dsregcmd /leave* e **pressione Enter**.</span><span class="sxs-lookup"><span data-stu-id="c78d9-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="c78d9-111">Quando estiver concluído, escreva *dsregcmd /junte* e prima **Enter**.</span><span class="sxs-lookup"><span data-stu-id="c78d9-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="c78d9-112">Quando estiver concluído, feche o pedido de comando.</span><span class="sxs-lookup"><span data-stu-id="c78d9-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="c78d9-113">Reinicie o computador e entre no OneDrive.</span><span class="sxs-lookup"><span data-stu-id="c78d9-113">Reboot the computer, and log into OneDrive.</span></span>