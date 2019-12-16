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
ms.openlocfilehash: 33e94eac6a2982b8036e13d17bf60015f244f2cb
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053236"
---
# <a name="encrypt-email-messages-in-outlook"></a>Criptografar mensagens de e-mail no Outlook

A criptografia de mensagens do Office 365 é construída no Microsoft Azure Rights Management (Azure RMS), que faz parte da Proteção de Informações do Azure. Se sua assinatura incluir a Gestão de Direitos Do Azure ou a Proteção de Informações do Azure, **você não precisará tomar nenhuma ação para ativar ou ativar manualmente** o Serviço de Gerenciamento de Direitos.

Com base no feedback do cliente, não estaremos mais permitindo que as regras de fluxo de e-mail da Exchange criptografem automaticamente o e-mail de saída contendo determinado tipo de informação sensível em seu locatário por padrão. Em vez disso, estamos fornecendo instruções detalhadas sobre como você pode fazê-lo sozinhos. Para obter detalhes adicionais sobre como criar uma regra de transporte para criptografar informações confidenciais, consulte [este artigo.](https://aka.ms/OmeEtr)

- Se estiver usando o Outlook na Web (anteriormente **OWA):** Ao compor uma mensagem de e-mail, basta clicar em **Proteger** na OWA. Isso aplicará a permissão "Não encaminhe". Clique **na permissão de alteração** e escolha **criptografar** apenas a mensagem.

- Se estiver usando o **cliente do Outlook:** Para enviar uma mensagem criptografada do Outlook 2013 ou 2016, ou Outlook 2016 para Mac, selecione**Permissões**de **Opções** > e selecione a opção de proteção de que precisa.

- Para **criptografar automaticamente todos os e-mails** enviados a determinados destinatários ou organizações parceiras externas, você precisa criar uma regra de transporte de fluxo de correio no Exchange Admin Center. Instruções detalhadas são fornecidas [neste artigo de suporte.](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities)

