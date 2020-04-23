---
title: Recordar ou substituir uma mensagem de e-mail
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: e541620a499b02a7206579ffcc505ceb4e632a4c
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742766"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Lembre-se ou substitua uma mensagem de e-mail no Microsoft 365

- Só se **pode recordar mensagens que são enviadas a pessoas da sua organização.** Se a mensagem foi enviada para um endereço gmail, por exemplo, não se lembra.
- Só é **possível recordar mensagens enviadas do Outlook 2016 para pc**. Se um utilizador enviar uma mensagem usando o Outlook para Mac ou Outlook na web, não pode recordá-la.
- Se for administrador, pode **recordar mensagens em nome dos utilizadores utilizando o PowerShell**. Não se pode lembrar de mensagens do centro de administração. Desloque-se para "Procurar e apagar mensagens de correio eletrónico na sua organização" para obter mais informações.

**Lembre-se ou substitua uma mensagem de e-mail que enviou**

1. No painel de pastas à esquerda da janela Outlook, escolha a pasta Itens Enviados.
2. Abra a mensagem que quer recordar. Tem de clicar duas vezes para abrir a mensagem. Selecionando a mensagem para que apareça no painel de leitura não lhe permitirá recordar a mensagem.
3. A partir do separador Mensagem, selecione **Ações** > **Recordar Esta Mensagem**.
4. Escolha **Eliminar cópias não lidas desta mensagem** ou eliminar **cópias não lidas e substituir por uma nova mensagem**e, em seguida, selecione **OK**.
5. Se estiver a enviar uma mensagem de substituição, componha a mensagem e, em seguida, selecione **Enviar**.
6. O sucesso ou falha de uma recolha de mensagens depende das definições dos destinatários no Outlook.

Para mais informações, incluindo como verificar a recolha, consulte Recordar ou substituir uma mensagem de [e-mail que enviou](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

***Procure e elimine mensagens de correio eletrónico na sua organização*** Para pesquisar e apagar mensagens de correio eletrónico na sua organização, é mais fácil se for um administrador global. Se não for um administrador global, a sua conta deve ser adicionada ao grupo de papel do eDiscovery Manager ou ao papel de gestão de Compliance Search. Para eliminar mensagens, terá de se juntar ao grupo de gestão da organização ou ao papel de gestão de Pesquisa e Purga. As permissões a estas funções são atribuídas no Centro de [Segurança & conformidade.](https://protection.office.com/)

1. [Crie uma pesquisa de conteúdo](https://docs.microsoft.com/office365/securitycompliance/content-search) para encontrar a mensagem para apagar.
2. [Ligue-se ao Centro de Conformidade de Segurança & PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps). 

Se estiver a utilizar o MFA, consulte [o Connect para a segurança Microsoft 365 & Compliance Center PowerShell utilizando a autenticação de vários fatores](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps). 
