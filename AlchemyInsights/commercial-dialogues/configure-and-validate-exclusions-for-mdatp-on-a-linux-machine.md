---
title: Configure e valide exclusões para MDATP numa máquina Linux
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4fad0a513f7c6d2f0337019488a4055c25e1650d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749252"
---
# <a name="configure-and-validate-exclusions-for-mdatp-on-a-linux-machine"></a><span data-ttu-id="b373a-102">Configure e valide exclusões para MDATP numa máquina Linux</span><span class="sxs-lookup"><span data-stu-id="b373a-102">Configure and validate exclusions for MDATP on a Linux machine</span></span>

<span data-ttu-id="b373a-103">Pode excluir certos ficheiros, pastas, processos e ficheiros abertos a processos a partir de digitalizações de MDATP.</span><span class="sxs-lookup"><span data-stu-id="b373a-103">You can exclude certain files, folders, processes, and process-opened files from MDATP scans.</span></span> <span data-ttu-id="b373a-104">As exclusões ajudam a prevenir a deteção incorreta de software e ficheiros únicos ou personalizados para a sua organização.</span><span class="sxs-lookup"><span data-stu-id="b373a-104">Exclusions help prevent incorrect detection of software and files unique or customized to your organization.</span></span> <span data-ttu-id="b373a-105">As exclusões também ajudam a mitigar os problemas de desempenho causados pelo MDATP.</span><span class="sxs-lookup"><span data-stu-id="b373a-105">Exclusions also help mitigate performance problems caused by MDATP.</span></span>

<span data-ttu-id="b373a-106">Para saber mais, consulte [Configure e valide exclusões para MDATP para Linux](https://go.microsoft.com/fwlink/?linkid=2144517).</span><span class="sxs-lookup"><span data-stu-id="b373a-106">To learn more, see [Configure and validate exclusions for MDATP for Linux](https://go.microsoft.com/fwlink/?linkid=2144517).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="b373a-107">As exclusões descritas neste artigo não se aplicam a outras capacidades de MDATP para o Linux, incluindo a deteção e resposta de pontos finais (EDR).</span><span class="sxs-lookup"><span data-stu-id="b373a-107">The exclusions described in this article don't apply to other capabilities of MDATP for Linux, including endpoint detection and response (EDR).</span></span> <span data-ttu-id="b373a-108">Os ficheiros que exclui utilizando os métodos descritos neste artigo podem ainda desencadear alertas EDR e outras capacidades de deteção.</span><span class="sxs-lookup"><span data-stu-id="b373a-108">Files that you exclude by using the methods described in this article can still trigger EDR alerts and other detection capabilities.</span></span>
