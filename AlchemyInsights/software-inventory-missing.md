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
# <a name="software-inventory-is-missing-or-inaccurate"></a>O inventário de software está em falta ou incorreto

O inventário de software no Gestão de Vulnerabilidades e Ameaças (TVM) é uma lista de software conhecido na sua organização com Enumerações da Plataforma Comuns oficial (CPE).

Os produtos de software sem um CPE oficial não têm vulnerabilidades publicadas. O inventário também inclui detalhes como o nome do fornecedor, o número de fracos, ameaças e o número de dispositivos expostos.

Normalmente, as alterações de software nos dispositivos refletem-se nos portais de segurança no prazo de duas horas. No entanto, por vezes pode demorar mais tempo. De momento, não existe nenhuma forma de forçar uma sincronização; esta é uma avaliação contínua contínua.

Se fez uma alteração de software e a alteração não for refletida corretamente na TVM ao fim de 5 horas, siga estes passos:

1. Consulte a secção de provas de software para compreender como o software foi detetado.
1. Certifique-se de que o software é suportado. O software pode estar visível apenas ao nível do dispositivo, mesmo que não seja atualmente suportado pela Gestão de Vulnerabilidades e Ameaças. No entanto, apenas estão disponíveis dados limitados.
1. Para ver os passos para comunicar a incorretaidade do portal, consulte [Relatório incorreto.](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy)
   
    **Nota:** comunicar uma imprecisão a partir do portal MDE é um canal de um sentido para a engenharia. Se o problema for urgente, abra um pedido de suporte.

Para obter mais informações, consulte [Inventário de software - Gestão de Vulnerabilidades e Ameaças](/microsoft-365/security/defender-endpoint/tvm-software-inventory).