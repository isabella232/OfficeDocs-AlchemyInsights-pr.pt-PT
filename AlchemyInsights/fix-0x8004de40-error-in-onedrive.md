---
title: Corrigir erro 0x8004de40 no OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: b9bd6dff48f78063e3d47f5fe2f834f59eb9868a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745141"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="dc12e-102">Corrigir erro 0x8004de40 no OneDrive</span><span class="sxs-lookup"><span data-stu-id="dc12e-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="dc12e-103">Se receber um erro de 0x8004de40 com o OneDrive:</span><span class="sxs-lookup"><span data-stu-id="dc12e-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="dc12e-104">Reinicie o computador afetado enquanto estiver ligado ao seu domínio acitve Directory.</span><span class="sxs-lookup"><span data-stu-id="dc12e-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="dc12e-105">Se um reboot não corrigir o problema, un un unin e rejoine o seu dispositivo a partir de Azure AD.</span><span class="sxs-lookup"><span data-stu-id="dc12e-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="dc12e-106">**Nota:** Deve estar na sua rede corporativa durante a realização destes passos.</span><span class="sxs-lookup"><span data-stu-id="dc12e-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="dc12e-107">Não execute estes passos quando não é capaz de se conectar à sua infraestrutura corporativa (por exemplo, durante a viagem).</span><span class="sxs-lookup"><span data-stu-id="dc12e-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="dc12e-108">Abra um pedido de comando elevado.</span><span class="sxs-lookup"><span data-stu-id="dc12e-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="dc12e-109">Para abrir um pedido de comando elevado, clique em - **Iniciar**, clique com o botão direito **Command Prompt**e, em seguida, clique em Executar **como administrador**.</span><span class="sxs-lookup"><span data-stu-id="dc12e-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="dc12e-110">Tipo *dsregcmd /leave* and press **Enter**.</span><span class="sxs-lookup"><span data-stu-id="dc12e-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="dc12e-111">Quando estiver concluído, *escreva /junte-se* e prima **Enter**.</span><span class="sxs-lookup"><span data-stu-id="dc12e-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="dc12e-112">Quando estiver completo, feche o aviso de comando.</span><span class="sxs-lookup"><span data-stu-id="dc12e-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="dc12e-113">Reinicie o computador e inicie sessão no OneDrive.</span><span class="sxs-lookup"><span data-stu-id="dc12e-113">Reboot the computer, and log into OneDrive.</span></span>