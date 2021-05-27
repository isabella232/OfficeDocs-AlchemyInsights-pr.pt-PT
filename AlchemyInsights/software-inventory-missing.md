---
title: O inventário de software está em falta ou incorreto
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11382"
- "9001470"
ms.openlocfilehash: e886a53f8c063b5395dd002a7d16186985584d72
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/26/2021
ms.locfileid: "52676511"
---
# <a name="software-inventory-is-missing-or-inaccurate"></a><span data-ttu-id="f4e0e-102">O inventário de software está em falta ou incorreto</span><span class="sxs-lookup"><span data-stu-id="f4e0e-102">Software inventory is missing or inaccurate</span></span>

<span data-ttu-id="f4e0e-103">O inventário de software no Gestão de Vulnerabilidades e Ameaças (TVM) é uma lista de software conhecido na sua organização com Enumerações da Plataforma Comuns oficial (CPE).</span><span class="sxs-lookup"><span data-stu-id="f4e0e-103">The software inventory in threat and vulnerability management (TVM) is a list of known software in your organization with official Common Platform Enumerations (CPE).</span></span>

<span data-ttu-id="f4e0e-104">Os produtos de software sem um CPE oficial não têm vulnerabilidades publicadas.</span><span class="sxs-lookup"><span data-stu-id="f4e0e-104">Software products without an official CPE don’t have vulnerabilities published.</span></span> <span data-ttu-id="f4e0e-105">O inventário também inclui detalhes como o nome do fornecedor, o número de fracos, ameaças e o número de dispositivos expostos.</span><span class="sxs-lookup"><span data-stu-id="f4e0e-105">The inventory also includes details such as the name of the vendor, number of weaknesses, threats, and number of exposed devices.</span></span>

<span data-ttu-id="f4e0e-106">Normalmente, as alterações de software nos dispositivos refletem-se nos portais de segurança no prazo de duas horas.</span><span class="sxs-lookup"><span data-stu-id="f4e0e-106">Software changes on devices are typically reflected in security portals within two hours.</span></span> <span data-ttu-id="f4e0e-107">No entanto, por vezes pode demorar mais tempo.</span><span class="sxs-lookup"><span data-stu-id="f4e0e-107">However, it may sometimes take longer.</span></span> <span data-ttu-id="f4e0e-108">De momento, não existe nenhuma forma de forçar uma sincronização; esta é uma avaliação contínua contínua.</span><span class="sxs-lookup"><span data-stu-id="f4e0e-108">There’s currently no way to force a sync; this is an ongoing continuous assessment.</span></span>

<span data-ttu-id="f4e0e-109">Se fez uma alteração de software e a alteração não for refletida corretamente na TVM ao fim de 5 horas, siga estes passos:</span><span class="sxs-lookup"><span data-stu-id="f4e0e-109">If you made a software change and the change is not accurately reflected in TVM after 5 hours, follow these steps:</span></span>

1. <span data-ttu-id="f4e0e-110">Consulte a secção de provas de software para compreender como o software foi detetado.</span><span class="sxs-lookup"><span data-stu-id="f4e0e-110">Check the software evidence section to understand how the software was detected.</span></span>
1. <span data-ttu-id="f4e0e-111">Certifique-se de que o software é suportado.</span><span class="sxs-lookup"><span data-stu-id="f4e0e-111">Make sure that the software is supported.</span></span> <span data-ttu-id="f4e0e-112">O software pode estar visível apenas ao nível do dispositivo, mesmo que não seja atualmente suportado pela Gestão de Vulnerabilidades e Ameaças.</span><span class="sxs-lookup"><span data-stu-id="f4e0e-112">Software may be visible only at the device level even if it is currently not supported by threat and vulnerability management.</span></span> <span data-ttu-id="f4e0e-113">No entanto, apenas estão disponíveis dados limitados.</span><span class="sxs-lookup"><span data-stu-id="f4e0e-113">However, only limited data is available.</span></span>
1. <span data-ttu-id="f4e0e-114">Para ver os passos para comunicar a incorretaidade do portal, consulte [Relatório incorreto.](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy)</span><span class="sxs-lookup"><span data-stu-id="f4e0e-114">For steps to report the inaccuracy from the portal, see [Report inaccuracy](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy).</span></span>
   
    <span data-ttu-id="f4e0e-115">**Nota:** comunicar uma imprecisão a partir do portal MDE é um canal de um sentido para a engenharia.</span><span class="sxs-lookup"><span data-stu-id="f4e0e-115">**Note**: Reporting an inaccuracy from the MDE portal is a one-way channel to engineering.</span></span> <span data-ttu-id="f4e0e-116">Se o problema for urgente, abra um pedido de suporte.</span><span class="sxs-lookup"><span data-stu-id="f4e0e-116">If the issue is urgent, open a support ticket.</span></span>

<span data-ttu-id="f4e0e-117">Para obter mais informações, consulte [Inventário de software - Gestão de Vulnerabilidades e Ameaças](/microsoft-365/security/defender-endpoint/tvm-software-inventory).</span><span class="sxs-lookup"><span data-stu-id="f4e0e-117">For more information, see [Software inventory - threat and vulnerability management](/microsoft-365/security/defender-endpoint/tvm-software-inventory).</span></span>