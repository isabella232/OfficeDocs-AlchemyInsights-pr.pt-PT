---
title: S/MIME do Outlook na web
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: f2c047ca31c586c0aa36701e6e7ca9976cfd1734
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666851"
---
# <a name="encrypt-email-messages-in-outlook"></a>Encriptar mensagens de correio electrónico no Outlook

Encriptação de mensagens do Office 365 foi criada no Microsoft Azure gestão de direitos (Azure RMS), que faz parte da protecção de informações de Azure. Se a subscrição inclui a gestão de direitos Azure ou protecção de informações Azure, **não é necessário efectuar quaisquer acções para activar manualmente ou activar** o serviço de gestão de direitos.

Com base nos comentários dos clientes, a Microsoft já não activar regras de fluxo de correio Exchange encriptar automaticamente correio electrónico enviado com determinado tipo de informações sensíveis no seu tenant por predefinição. Em vez disso, estamos a fornecer instruções detalhadas sobre como pode fazê-lo mitos. Para obter detalhes adicionais sobre como criar uma regra de transporte para encriptar informações sensíveis, consulte [Este artigo](https://aka.ms/OmeEtr).

- Se utilizar o Outlook na Web (anteriormente **OWA**): quando estiver a compor uma mensagem de correio electrónico, basta clicar **proteger** no OWA. Isto aplicará a permissão "Não reencaminhar". Clique em **Alterar permissão** e escolher **encriptar** apenas a encriptar a mensagem.

- Se utilizar o **cliente Outlook**: para enviar uma mensagem encriptada a partir do Outlook 2013 ou de 2016, ou de 2016 do Outlook para Mac, seleccione **Opções** > **permissões**, em seguida, seleccione a opção de protecção que necessita.

- Para **encriptar automaticamente todas as mensagem de correio electrónico** enviadas para determinados destinatários ou organizações de parceiro externo, é necessário criar uma regra de transporte de fluxo de correio no Centro de administração do Exchange. São fornecidas instruções detalhadas no [presente artigo de suporte](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).

