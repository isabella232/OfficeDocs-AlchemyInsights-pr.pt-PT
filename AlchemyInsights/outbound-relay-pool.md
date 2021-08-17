---
title: Grupo de relay de saída
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "12315"
ms.openlocfilehash: d2f83b3afc4abf72a3e18bffe5ac9d6c940cc216916925338c18f0fb8a39948a
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/11/2021
ms.locfileid: "57883142"
---
# <a name="outbound-relay-pool"></a>Grupo de relay de saída

A Microsoft está a fazer algumas alterações à configuração do relaying ou encaminhamento de e-mail através Microsoft 365. As mensagens em determinados cenários são re encaminhadas ou relayadas através Microsoft 365 através de um grupo de relay especial. As mensagens enviadas através do grupo de relay podem aparecer na pasta de e-mail de lixo do destinatário. Para obter mais informações, consulte [ações de entrega de saída](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)

Para evitar um cenário com o grupo de reenainhamento, certifique-se de que as mensagens reencainhadas/reencainhadas cumprem um dos seguintes critérios:

- O remetente de saída é um domínio aceite do inquilino.
- O SPF (Sender Policy Framework) passa quando a mensagem é recebida Microsoft 365.
- O DKIM (DomainKeys Identified Mail) no domínio do remetente P2 passa quando a mensagem é enviada para Microsoft 365.
 
As mensagens que cumprem os critérios descritos acima não são reencalecidas através do grupo de reenais.

Se o registo MX do seu domínio estiver apontado para um servidor de terceiros ou no local, utilize a filtragem melhorada para se certificar de que a validação de SPF está correta para o e-mail de entrada e para evitar o envio de e-mails através do agrupamento de relay.

**Como podemos saber se estamos a ser afetados pelo grupo de relay?**

Se os seus e-mails re encaminhados ou re encaminhados utilizarem um dos critérios acima, as mensagens não serão relayadas através do grupo de relay. No entanto, se uma mensagem for enviada através de um conjunto de relay, o IP do servidor de saída está no intervalo 40.95.0.0/16 e o nome do servidor de saída inclui **rly** no nome.

