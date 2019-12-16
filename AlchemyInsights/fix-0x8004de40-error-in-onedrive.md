---
title: Corrigir erro 0x8004de40 no OneDrive
ms.author: pebaum
author: pebaum
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 48b29f57763ca22a71a23b2afddcac0e8e8a95db
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052048"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="266c3-102">Corrigir erro 0x8004de40 no OneDrive</span><span class="sxs-lookup"><span data-stu-id="266c3-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="266c3-103">Se você receber um erro 0x8004de40 com OneDrive:</span><span class="sxs-lookup"><span data-stu-id="266c3-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="266c3-104">Reiniciar o computador afetado enquanto estiver conectado ao seu domínio acitve diretório.</span><span class="sxs-lookup"><span data-stu-id="266c3-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="266c3-105">Se uma reinicialização não corrigir o problema, unjoin e voltar ao seu dispositivo a partir de AD Azure.</span><span class="sxs-lookup"><span data-stu-id="266c3-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="266c3-106">**Nota:** Você deve estar em sua rede corporativa durante a execução dessas etapas.</span><span class="sxs-lookup"><span data-stu-id="266c3-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="266c3-107">Não execute essas etapas quando você não é capaz de se conectar à sua infraestrutura corporativa (por exemplo, durante a viagem).</span><span class="sxs-lookup"><span data-stu-id="266c3-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="266c3-108">Abra uma alerta de comando elevado.</span><span class="sxs-lookup"><span data-stu-id="266c3-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="266c3-109">Para abrir um alerta de comando elevado, clique em - **Comece,** clique à direita **no Comando Prompt**e, em seguida, clique em Correr como **administrador.**</span><span class="sxs-lookup"><span data-stu-id="266c3-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="266c3-110">Tipo *dsregcmd /leave* and press **Enter**.</span><span class="sxs-lookup"><span data-stu-id="266c3-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="266c3-111">Quando completo, tipo *dsregcmd /join* e **pressione Entre.**</span><span class="sxs-lookup"><span data-stu-id="266c3-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="266c3-112">Quando estiver completo, feche o alerta de comando.</span><span class="sxs-lookup"><span data-stu-id="266c3-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="266c3-113">Reiniciar o computador, e entrar em OneDrive.</span><span class="sxs-lookup"><span data-stu-id="266c3-113">Reboot the computer, and log into OneDrive.</span></span>