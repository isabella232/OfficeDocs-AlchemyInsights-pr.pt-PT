---
title: S/MIME em Outlook na web
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 6bbbf8722dacb8b7d5191d57ce1055a48dcb4dd0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511519"
---
# <a name="encrypt-email-messages-in-outlook"></a>Criptografe mensagens de e-mail no Outlook

A Encriptação de Mensagens Microsoft 365 é construída na Microsoft Azure Rights Management (Azure RMS), que faz parte da Azure Information Protection. Se a sua subscrição incluir Azure Rights Management ou Azure Information Protection, **não precisa de tomar quaisquer ações para ativar ou ativar manualmente** o Serviço de Gestão de Direitos.

Com base no feedback do cliente, deixaremos de permitir que as regras de fluxo de correio exchange possam encriptar automaticamente o e-mail de saída contendo determinado tipo de informação sensível no seu inquilino por padrão. Em vez disso, estamos a fornecer instruções detalhadas sobre como podem fazê-lo. Para obter mais detalhes sobre como criar uma regra de transporte para encriptar informações confidenciais, consulte [este artigo](https://aka.ms/OmeEtr).

- Se utilizar o Outlook na Web (anteriormente **OWA**): Ao compor uma mensagem de correio eletrónico, basta clicar em **Protect** in OWA. Isto aplica-se a permissão "Não encaminhar". Clique **na permissão De alterar** e escolha **Criptografar** apenas para encriptar a mensagem.

- Se utilizar **o cliente Outlook**: Para enviar uma mensagem encriptada do Outlook 2013 ou 2016, ou do Outlook 2016 para Mac, selecione **Permissões de**  >  **Opções**, então selecione a opção de proteção de que necessita.

- Para **encriptar automaticamente todos os e-mails** enviados a determinados destinatários ou organizações parceiras externas, é necessário criar uma regra de transporte de fluxo de correio no Exchange Admin Center. São fornecidas instruções detalhadas [neste artigo de apoio.](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities)

