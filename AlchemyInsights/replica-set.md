---
title: Conjunto de réplica
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 3834696ff59b7e96e90a5b660a489003dfa9729c
ms.sourcegitcommit: 581c696ec108184adae9d4bc8f47cb9247131de8
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714254"
---
# <a name="replica-set"></a><span data-ttu-id="b6117-102">Conjunto de réplica</span><span class="sxs-lookup"><span data-stu-id="b6117-102">Replica set</span></span>

<span data-ttu-id="b6117-103">O AADDS também é chamado como o domínio gerido.</span><span class="sxs-lookup"><span data-stu-id="b6117-103">AADDS is also called as the managed domain.</span></span> <span data-ttu-id="b6117-104">Na verdade, são dois controladores de domínio que são executados e mantidos pelo backend.</span><span class="sxs-lookup"><span data-stu-id="b6117-104">It is actually two domain controllers that are run and maintained by the backend.</span></span> <span data-ttu-id="b6117-105">Os dois DCs incluem um DC principal e um DC de replicação.</span><span class="sxs-lookup"><span data-stu-id="b6117-105">The two DCs include one main DC and one replication DC.</span></span> <span data-ttu-id="b6117-106">As cópias de segurança em AADDS (domínio gerido) são um processo automatizado gerido pela plataforma Azure.</span><span class="sxs-lookup"><span data-stu-id="b6117-106">Backups in AADDS (managed domain) are an automated process managed by the Azure platform.</span></span> <span data-ttu-id="b6117-107">Em caso de problema com o seu domínio gerido, o suporte Azure pode ajudá-lo a restaurar a partir de backup.</span><span class="sxs-lookup"><span data-stu-id="b6117-107">In the event of an issue with your managed domain, Azure support can assist you in restoring from backup.</span></span>

<span data-ttu-id="b6117-108">Cria-se cada conjunto de réplicas numa rede virtual.</span><span class="sxs-lookup"><span data-stu-id="b6117-108">You create each replica set in a virtual network.</span></span> <span data-ttu-id="b6117-109">Cada rede virtual deve ser espreitada para todas as outras redes virtuais que hospedam um conjunto de réplicas de domínio gerido.</span><span class="sxs-lookup"><span data-stu-id="b6117-109">Each virtual network must be peered to every other virtual network that hosts a managed domain's replica set.</span></span> <span data-ttu-id="b6117-110">Esta configuração cria uma topologia de rede de malha que suporta a replicação do diretório.</span><span class="sxs-lookup"><span data-stu-id="b6117-110">This configuration creates a mesh network topology that supports directory replication.</span></span> <span data-ttu-id="b6117-111">Uma rede virtual pode suportar vários conjuntos de réplicas, desde que cada conjunto de réplicas esteja numa sub-rede virtual diferente.</span><span class="sxs-lookup"><span data-stu-id="b6117-111">A virtual network can support multiple replica sets, provided that each replica set is in a different virtual subnet.</span></span>

<span data-ttu-id="b6117-112">Para obter mais detalhes sobre o conjunto de [réplicas, consulte os conjuntos de réplicas de conceitos.](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets)</span><span class="sxs-lookup"><span data-stu-id="b6117-112">For more details on Replica set, see [Concepts Replica sets](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).</span></span>
