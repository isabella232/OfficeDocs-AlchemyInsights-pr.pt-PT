---
title: Outlook Desktop recall ou substituir uma mensagem de e-mail
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
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/25/2019
ms.locfileid: "36496122"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Lembre-se ou substitua uma mensagem de e-mail do Outlook

- Como administrador, você pode **recordar mensagens em nome dos usuários usando powershell**. Você não pode se lembrar de mensagens do centro de administração.
- Você só pode **recordar mensagens que são enviadas para as pessoas em sua organização**. Se a mensagem foi enviada para um endereço do Gmail, por exemplo, você não pode se lembrar.
- Você só pode **recordar as mensagens enviadas do Outlook 2016 no PC**. Se um usuário enviar uma mensagem usando o Outlook para Mac ou Outlook na web, você não pode se lembrar.

Para recordar ou substituir uma mensagem de e-mail:

1. No painel de pasta à esquerda da janela do Outlook, selecione a pasta Sent Items.
1. Clique duas vezes na mensagem que deseja recordar para abri-la.
1. Selecione a guia **mensagem** e, em seguida, selecione **ações** > **lembrem essa mensagem**.
1. Selecione **excluir cópias não lidas desta mensagem** ou excluir **cópias não lidas e substituir por uma nova mensagem,** e, em seguida, selecione **OK**.
1. Se você estiver enviando uma mensagem de substituição, componha a mensagem e selecione **envie.**
1. O sucesso ou o fracasso de um recall de mensagens depende das configurações do destinatário no Outlook. Para que as etapas verific na recordação, veja [este artigo.](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)

Pesquise e exclua mensagens de e-mail em sua organização

- Se você não for um administrador global, sua conta deve ser adicionada à função do gerente do eDiscovery ou à função de gerenciamento de pesquisa de conformidade para pesquisar mensagens. Para excluir mensagens, você precisará participar do grupo de função da Organização Gerencial ou da função de gerenciamento de Pesquisa e Expurgo. As permissões para essas funções são atribuídas no centro de [segurança e conformidade.](https://go.microsoft.com/fwlink/?linkid=2083731)
- [Crie uma pesquisa de conteúdo](https://docs.microsoft.com/office365/securitycompliance/content-search) para encontrar a mensagem para excluir.
- [Conecte-se ao PowerShell do Centro](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)de Segurança e Conformidade.

Se você estiver usando a autenticação multifator, [consulte o Connect to Office 365 Security and Compliance Center PowerShell usando autenticação multifator.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)