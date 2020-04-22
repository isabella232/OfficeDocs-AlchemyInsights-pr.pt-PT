---
title: Outlook Desktop recordar ou substituir uma mensagem de e-mail
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: d64332778f9132aff6a9660bb0d522f4e16b753c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687521"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Lembre-se ou substitua uma mensagem de e-mail do Outlook

- Como administrador, pode **recordar mensagens em nome dos utilizadores que utilizam o PowerShell**. Não se pode lembrar de mensagens do centro de administração.
- Só se **pode recordar mensagens que são enviadas a pessoas da sua organização.** Se a mensagem foi enviada para um endereço gmail, por exemplo, não se lembra.
- Só é **possível recordar mensagens enviadas do Outlook 2016 no PC**. Se um utilizador enviar uma mensagem usando o Outlook para Mac ou Outlook na web, não pode recordá-la.

Para recordar ou substituir uma mensagem de e-mail:

1. No painel de pastas à esquerda da janela Outlook, selecione a pasta Itens Enviados.
1. Clique duas vezes na mensagem que pretende recordar para abri-la.
1. Selecione o separador **Mensagem** e, em seguida, selecione **Ações** > **Recall This Message**.
1. **Selecione Eliminar cópias não lidas desta mensagem** ou eliminar **cópias não lidas e substituir por uma nova mensagem**, e, em seguida, selecione **OK**.
1. Se estiver a enviar uma mensagem de substituição, componha a mensagem e, em seguida, selecione **Enviar**.
1. O sucesso ou falha de uma recolha de mensagens depende das definições do destinatário no Outlook. Para que os passos para verificar a recolha, consulte [este artigo](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Procure e elimine mensagens de correio eletrónico na sua organização

- Se não for um administrador global, a sua conta deve ser adicionada ao papel do eDiscovery Manager ou ao papel de gestão da Procura de Compliance Search para procurar mensagens. Para eliminar mensagens, terá de se juntar ao grupo de gestão da organização ou ao papel de gestão de Pesquisa e Purga. As permissões para estas funções são atribuídas no Centro de [Segurança e Conformidade.](https://go.microsoft.com/fwlink/?linkid=2083731)
- [Crie uma pesquisa de conteúdo](https://docs.microsoft.com/office365/securitycompliance/content-search) para encontrar a mensagem para apagar.
- [Ligue-se ao PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)do Centro de Segurança e Conformidade.

Se estiver a utilizar a autenticação de vários fatores, consulte [o Connect to Microsoft 365 security and Compliance Center PowerShell utilizando a autenticação de vários fatores](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).