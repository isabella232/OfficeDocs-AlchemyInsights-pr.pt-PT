---
title: Vários objetos têm o mesmo endereço de e-mail que identidade
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: cc932aa7ecbd1e338c409a7a6525e2c4e673b232
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439714"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a>Vários objetos têm o mesmo endereço de e-mail que identidade

**Objetos múltiplos**

Uma das razões comuns deste erro é não ser capaz de encaminhar um pedido do Outlook Web Access corretamente na presença de vários objetos com o mesmo endereço de e-mail que a identidade. Para encontrar estes objetos, executar os seguintes comandos:

· Get-Recipient<email address>

· Get-User<email address>

· Get-User <email address> -SoftDeletedUser

· Obter Contacto<email address>

· Get-Mailbox <email address> -PublicFolder

· Get-Mailbox <email address> -IncludeSoftDeletedMailbox

· Get-Mailbox <email address> -InactiveMailboxOnly

Para resolver o problema, remova vários objetos com a mesma identidade de e-mail e certifique-se de que existe um único objeto com a identidade específica do e-mail e que o seu tipo de destinatário é userMailbox.

**O mesmo endereço é usado para caixas de correio de negócios e consumidores**

Outra das causas é quando o mesmo endereço é usado para caixas de correio de empresas e consumidores. Neste caso, o utilizador deve alterar o seu pseudónimo principal de consumidor até que o Café suporte este cenário. Trata-se de um erro permanente que não desaparece sem intervenção.

Para mais informações, consulte [alterar o endereço de e-mail ou o número de telefone da sua conta Microsoft.](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account)