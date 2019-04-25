---
title: Resgate de ambiente de trabalho do Outlook ou substituir uma mensagem de correio electrónico
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: aced684777ef82860b969aea8825699b78b04c5a
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32389752"
---
# <a name="recall-or-replace-an-email-message"></a>Resgatar ou substituir uma mensagem de correio electrónico

- Como administrador, pode de **resgate de mensagens em nome dos utilizadores utilizando o PowerShell**. Não é possível recuperar mensagens a partir do Centro de administração.
- Pode **apenas mensagens de recuperação que são enviadas para pessoas na organização**. Se a mensagem foi enviada para um endereço de Gmail, por exemplo, não se lembrá-lo.
- Pode **apenas resgatar as mensagens enviadas de 2016 do Outlook no computador**. Se um utilizador envia uma mensagem utilizando o Outlook para Mac ou o Outlook na web, não se lembrá-lo.

Para resgatar ou substituir uma mensagem de correio electrónico:

1. No painel de pastas do lado esquerdo da janela do Outlook, seleccione a pasta Itens enviados.
1. Faça duplo clique sobre a mensagem que pretende recuperar para o abrir.
1. Seleccione o separador de **mensagem** e, em seguida, seleccione **Acções** > **Resgatar a mensagem**.
1. Seleccione **Eliminar cópias não lidas desta mensagem** ou **elimine cópias não lidas e substitua por uma nova mensagem**e, em seguida, seleccione **' OK '**.
1. Se estiver a enviar uma mensagem de substituição, compor a mensagem e, em seguida, seleccione **Enviar**.
1. O êxito ou falha do resgate de mensagens depende de definições do destinatário do Outlook. Para obter passos verificar a recuperação, consulte [Este artigo](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Procure e elimine mensagens de correio electrónico na organização

- Se não for um administrador global, a conta deve ser adicionada à função de Gestor de detecção de dados electrónicos ou a função de gestão de conformidade Procurar para procurar mensagens. Para eliminar mensagens, terá de associar o grupo de funções de gestão da organização ou a função de gestão de procura e remover. Permissões para estas funções são atribuídas no [Centro de segurança e conformidade](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Criar um conteúdo de procura](https://docs.microsoft.com/office365/securitycompliance/content-search) para localizar a mensagem para eliminar.
- [Ligar a segurança e conformidade Centro PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Se estiver a utilizar autenticação multi-factores, consulte [ligar para a segurança do Office 365 e conformidade Centro PowerShell utilizando autenticação multi-factores](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).