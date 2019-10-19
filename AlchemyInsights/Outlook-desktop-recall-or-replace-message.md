---
title: Outlook desktop recordar ou substituir uma mensagem de e-mail
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 3d3a6c253317137b7069a978b907c97d61bf7313
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/18/2019
ms.locfileid: "36496122"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Recuperar ou substituir uma mensagem de email do Outlook

- Como administrador, você pode **recuperar mensagens em nome dos usuários usando o PowerShell**. Não é possível recuperar mensagens do centro de administração.
- Você **só pode recuperar mensagens que são enviadas para pessoas em sua organização**. Se a mensagem foi enviada para um endereço do Gmail, por exemplo, você não pode se lembrar dele.
- Você **só pode recuperar mensagens enviadas do Outlook 2016 no PC**. Se um usuário envia uma mensagem usando o Outlook para Mac ou Outlook na Web, você não pode se lembrar dele.

Para recordar ou substituir uma mensagem de e-mail:

1. No painel de pastas à esquerda da janela do Outlook, selecione a pasta Itens enviados.
1. Clique duas vezes na mensagem que você deseja recuperar para abri-la.
1. Selecione a guia **mensagem** e, em seguida, selecione **ações** > para**recuperar esta mensagem**.
1. Selecione **Excluir cópias não lidas desta mensagem** ou **Excluir cópias não lidas e substitua por uma nova mensagem**e, em seguida, selecione **OK**.
1. Se você estiver enviando uma mensagem de substituição, componha a mensagem e, em seguida, selecione **Enviar**.
1. O êxito ou falha de uma recordação de mensagem depende das definições do destinatário no Outlook. Para obter as etapas para verificar o recall, consulte [Este artigo](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Pesquisar e excluir mensagens de email em sua organização

- Se você não for um administrador global, sua conta deverá ser adicionada à função de Gerenciador de eDiscovery ou à função de gerenciamento de pesquisa de conformidade para procurar mensagens. Para excluir mensagens, você precisará ingressar no grupo de funções Gerenciamento da organização ou na função de gerenciamento de pesquisa e remoção. As permissões para essas funções são atribuídas no [centro de conformidade e segurança](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Crie uma pesquisa de conteúdo](https://docs.microsoft.com/office365/securitycompliance/content-search) para localizar a mensagem a ser excluída.
- [Conecte-se ao PowerShell do centro de conformidade e segurança](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Se você estiver usando a autenticação multifator, consulte [conectar-se ao PowerShell do centro de conformidade e segurança do Office 365 usando a autenticação multifator](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).