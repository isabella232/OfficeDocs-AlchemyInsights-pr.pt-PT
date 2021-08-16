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
ms.openlocfilehash: 8750c9036f258d9c5edc94bb027d564140bbd9914712cc1f25ff3abc3f4b9468
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54041597"
---
# <a name="outbound-relay-pool"></a>Grupo de relay de saída

A Microsoft está a fazer algumas alterações à configuração do relaying ou encaminhamento de e-mail através Microsoft 365. As mensagens em determinados cenários são re encaminhadas ou relayadas através Microsoft 365 através de um grupo de relay especial. As mensagens enviadas através do grupo de relay podem aparecer na pasta de e-mail de lixo do destinatário. Para obter mais informações, consulte [ações de entrega de saída](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)

Para evitar um cenário com o grupo de reenainhamento, certifique-se de que as mensagens reencainhadas/reencainhadas cumprem um dos seguintes critérios:

- O remetente de saída é um domínio aceite do inquilino.
- O SPF (Sender Policy Framework) passa quando a mensagem chega Microsoft 365.
- O DKIM (DomainKeys Identified Mail) no domínio do remetente P2 passa quando a mensagem é enviada Microsoft 365.
 
As mensagens que cumprem os critérios descritos acima não são reencalecidas através do grupo de reenais.

Se o registo MX do seu domínio estiver apontado para um servidor de terceiros ou no local, utilize a filtragem melhorada para se certificar de que a validação de SPF está correta para o e-mail de entrada e para evitar o envio de e-mail através do agrupamento de relay.

**Como podemos saber se estamos a ser afetados pelo grupo de relay?**

Se os seus e-mails re encaminhados ou re encaminhados utilizarem um dos critérios acima, as mensagens não serão relayadas através do grupo de relay. No entanto, se uma mensagem for enviada através de um conjunto de relay, o IP do servidor de saída está no intervalo 40.95.0.0/16 e o nome do servidor de saída inclui **rly** no nome.

