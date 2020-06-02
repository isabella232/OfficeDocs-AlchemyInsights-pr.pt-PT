---
title: Outlook Desktop recordação ou substitui uma mensagem de e-mail
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: bb84363ae7d3c91750d5de789c091c7cebbbedc2
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44502330"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Relembrou substituir uma mensagem de email do Outlook

- Como administrador, pode **recordar mensagens em nome dos utilizadores que utilizam o PowerShell**. Não se lembra das mensagens do centro de administração.
- Só se **pode recordar mensagens enviadas a pessoas da sua organização.** Se a mensagem foi enviada para um endereço Gmail, por exemplo, não se lembra.
- Só é **possível recordar as mensagens enviadas do Outlook 2016 no PC**. Se um utilizador enviar uma mensagem utilizando o Outlook for Mac ou Outlook na web, não se pode lembrar dela.

Para recordar ou substituir uma mensagem de e-mail:

1. No painel de pastas à esquerda da janela Outlook, selecione a pasta 'Itens Enviados'.
1. Clique duas vezes na mensagem que deseja recordar para abri-la.
1. Selecione o separador **Mensagem** e, em seguida, selecione **Ações**  >  **Relembrem esta mensagem**.
1. **Selecione Eliminar cópias não lidas desta mensagem** ou **eliminar cópias não lidas e substituir por uma nova mensagem**e, em seguida, selecione **OK**.
1. Se estiver a enviar uma mensagem de substituição, compõe a mensagem e, em seguida, selecione **Enviar**.
1. O sucesso ou falha de uma chamada de mensagem depende das definições do destinatário no Outlook. Para obter medidas para verificar a recolha, consulte [este artigo](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Procure e elimine mensagens de e-mail na sua organização

- Se não for administrador global, a sua conta tem de ser adicionada à função de Gestor de EDiscovery ou à função de gestão de Compliance Search para procurar mensagens. Para eliminar mensagens, terá de se juntar ao grupo de funções de Gestão da Organização ou à função de gestão de Pesquisa e Purga. As permissões para estas funções são atribuídas no [Centro de Segurança e Conformidade](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Crie uma pesquisa de conteúdo](https://docs.microsoft.com/microsoft-365/compliance/content-search) para encontrar a mensagem para eliminar.
- [Ligue-se ao Centro de Segurança e Conformidade PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Se estiver a utilizar a autenticação multi-factor, consulte [Connect to Microsoft 365 security and Compliance Center PowerShell utilizando a autenticação de vários fatores](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).