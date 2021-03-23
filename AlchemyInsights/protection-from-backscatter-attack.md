---
title: Proteção contra ataque de backscatter
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9779"
- "9005743"
ms.openlocfilehash: 8d9214fe2f5d55a21c72296421dd837d7f1d7e7d
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037175"
---
# <a name="protection-from-backscatter-attack"></a>Proteção contra ataque de backscatter

Backscatter é relatórios de não-entrega (também conhecidos como NDRs ou mensagens de ressalto) que recebe para mensagens que não enviou. Os spammers falsificam (spoof) o **From:** endereço das suas mensagens, e muitas vezes usam endereços de e-mail reais para emprestar credibilidade às suas mensagens. Assim, quando os spammers enviam inevitavelmente mensagens a destinatários inexistentes, o servidor de e-mail de destino é essencialmente enganado para devolver a mensagem não entregue num NDR ao remetente forjado no endereço **From.**

Informações adicionais podem ser encontradas em [Backscatter em EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).

**Habilitar a proteção de backscatter**

Para ativar a proteção do backscatter, siga o caminho abaixo.

**Política de > de gestão de ameaças protection.office.com > > Antispam > Selecione a política de filtro de spam e edite a política > propriedades de spam > Mark como spam > > de backscatter NDR defini-lo para "On"**

Se acredita que uma conta foi comprometida, consulte o seguinte:

- [Respondendo a uma conta de e-mail comprometida](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)
- [Remoção de utilizadores bloqueados do portal Utilizadores Restritos no Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)



