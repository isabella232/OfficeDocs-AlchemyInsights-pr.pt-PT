---
title: S/MIME no Outlook na web
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 7184ffd68f56639a8bcb87e9c6cab88388868103
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764883"
---
# <a name="encrypt-email-messages-in-outlook"></a>Criptografe mensagens de e-mail no Outlook

A Encriptação de Mensagens Microsoft 365 é construída na Microsoft Azure Rights Management (Azure RMS), que faz parte da Proteção de Informação do Azure. Se a sua subscrição incluir a Azure Rights Management ou a Azure Information Protection, **não precisa de tomar quaisquer ações para ativar ou ativar manualmente** o Serviço de Gestão de Direitos.

Com base no feedback do cliente, deixaremos de permitir que as regras de fluxo de correio de troca criptografem automaticamente e-mails de saída contendo determinado tipo de informação sensível no seu inquilino por defeito. Em vez disso, estamos a dar instruções detalhadas sobre como podem fazê-lo a si mesmos. Para mais detalhes sobre como criar uma regra de transporte para encriptar informações sensíveis, consulte [este artigo](https://aka.ms/OmeEtr).

- Se utilizar o Outlook na Web (anteriormente **OWA**): Ao compor uma mensagem de e-mail, basta clicar em **Proteger** em OWA. Isto aplicará permissão "Não encaminhar". Clique na **permissão De alterar** e escolha **encriptar** apenas para encriptar a mensagem.

- Se utilizar o **cliente do Outlook**: Para enviar uma mensagem encriptada do Outlook 2013 ou 2016, ou do Outlook 2016 para Mac, selecione **Options** > **Permissions,** então selecione a opção de proteção de que necessita.

- Para **encriptar automaticamente todos os e-mails** enviados a determinados destinatários ou organizações parceiras externas, é necessário criar uma regra de transporte de fluxo de correio no Exchange Admin Center. Instruções detalhadas são fornecidas [neste artigo de apoio](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).

