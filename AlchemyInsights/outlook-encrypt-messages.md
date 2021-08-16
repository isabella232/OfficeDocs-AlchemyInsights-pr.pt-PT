---
title: S/MIME no Outlook na Web
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: bef87baafdbaf9346f99f1ff54aaa83bc9173c70f1412ea00afb717c15a8014c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54010735"
---
# <a name="encrypt-email-messages-in-outlook"></a>Encriptar mensagens de e-mail Outlook

Microsoft 365 A Encriptação de Mensagens é Microsoft Azure Gestão de Direitos (Azure RMS), que faz parte do Azure Information Protection. Se a sua subscrição incluir o Azure Rights Management ou o Azure Information Protection, não precisa de errar qualquer ação para ativar ou ativar **manualmente** o Serviço de Gestão de Direitos.

Com base nos comentários dos clientes, deixaremos de Exchange permitir que as regras de fluxo de correio encriptem automaticamente os e-mails enviados com determinados tipos de informações confidenciais no seu inquilino por predefinição. Em vez disso, fornecemos instruções detalhadas sobre como o pode fazer. Para obter detalhes adicionais sobre como criar uma regra de transporte para encriptar informações confidenciais, [consulte este artigo.](https://aka.ms/OmeEtr)

- Se estiver a Outlook na Web (anteriormente **OWA):** ao compor uma mensagem de e-mail, basta clicar **em** Proteger no OWA. Esta ação aplicará a permissão "Não re encaminhar". Clique em **Alterar permissão e selecionar** **Encriptar** para apenas encriptar a mensagem.

- Se estiver Outlook cliente: para enviar uma mensagem encriptado **a** partir do Outlook 2013 ou 2016 ou do Outlook 2016 para Mac, selecione Opções Permissões e, em seguida, selecione a opção de proteção de que  >  precisa.

- Para **encriptar** automaticamente todos os e-mails enviados para determinados destinatários ou organizações parceiras externas, tem de criar uma regra de transporte de fluxo de correio no centro de administração de Exchange de Correio. São fornecidas instruções detalhadas [neste artigo de suporte.](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities)

