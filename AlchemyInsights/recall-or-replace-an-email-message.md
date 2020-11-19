---
title: Relembrou substituir uma mensagem de e-mail
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 05016213a1387c5290cb5899359f1f10b5a413c0
ms.sourcegitcommit: 4e0ae808ee2a586339b396320e3edb8ba066a91a
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/19/2020
ms.locfileid: "49353517"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Relembrou substituir uma mensagem de e-mail na Microsoft 365

- Só se **pode recordar mensagens enviadas a pessoas da sua organização.** Por exemplo, se a mensagem foi enviada para um endereço Gmail, não se pode lembrar dela.
- Só é **possível recordar as mensagens enviadas do Outlook para o PC**. Se um utilizador enviar uma mensagem utilizando o Outlook for Mac ou Outlook na web, não se pode lembrar dela.
- Como administrador de inquilinos, pode **relembrá-lo em nome dos utilizadores utilizando o PowerShell** (Para mais informações, consulte: [Procure e elimine mensagens de correio de e-mail).](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)
- Não se lembra das mensagens do centro de administração. Desloque-se para "Procurar e apagar mensagens de correio na sua organização" para obter mais informações.

**Lembre-se ou substitua uma mensagem de e-mail que enviou**

1. No painel de pastas à esquerda da janela Outlook, escolha a pasta Itens Enviados.
2. Abra a mensagem que quer recordar. Tem de clicar duas vezes para abrir a mensagem. Selecionar a mensagem de modo a aparecer no painel de leitura não lhe permite recordar a mensagem.
3. A partir do separador Mensagem, selecione **Actions**  >  **Recall This Message**.
4. **Selecione Eliminar cópias não lidas desta mensagem** ou **eliminar cópias não lidas e substituir por uma nova mensagem** e, em seguida, selecione **OK**.
5. Se estiver a enviar uma mensagem de substituição, compõe a mensagem e, em seguida, selecione **Enviar**.
6. O sucesso ou falha de uma chamada de mensagem depende das definições dos destinatários no Outlook.

Para mais informações, incluindo como verificar a recolha, consulte [Recall ou substitua uma mensagem de e-mail que enviou.](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)

**_Para procurar e apagar mensagens de e-mail na sua organização,_** é mais fácil se for administrador global. Se não é administrador global, a sua conta tem de ser adicionada ao grupo de funções eDiscovery Manager ou à função de gestão compliance Search. Para eliminar mensagens, terá de se juntar ao grupo de funções de Gestão da Organização ou à função de gestão de Pesquisa e Purga. As permissões a estas funções são atribuídas no [Centro de Conformidade & de Segurança](https://protection.office.com/).

1. [Crie uma pesquisa de conteúdo](https://docs.microsoft.com/microsoft-365/compliance/content-search) para encontrar a mensagem para eliminar.
2. [Ligue-se ao Centro de Conformidade & PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).

Se estiver a utilizar o MFA (autenticação multi-factor), consulte [Connect to Microsoft 365 Security & Compliance Center PowerShell utilizando a autenticação de vários fatores](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).
