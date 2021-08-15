---
title: Ressartar ou substituir uma mensagem de e-mail
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
ms.openlocfilehash: 45882b49c5c47b3e0e4519e2339e6c68110bc75aebeaeac2d0ccd009bdfa3f7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54024397"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Ressarte ou substitua uma mensagem de e-mail Microsoft 365

- Só pode **ressaltar mensagens enviadas para pessoas na sua organização.** Por exemplo, se a mensagem tiver sido enviada para um endereço do Gmail, não se consegue recordar dela.
- Só pode **ressartar mensagens enviadas a partir Outlook para o PC.** Se um utilizador enviar uma mensagem através do Outlook para Mac ou Outlook na Web, não é possível ressambrar a mensagem.
- Como administrador inquilino, pode resgatar mensagens em nome dos utilizadores através do **PowerShell** (para obter mais informações, consulte: Procurar e eliminar mensagens de [e-mail).](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)
- Não é possível ressaltar mensagens a partir do centro de administração. Desloque-se para baixo até "Procurar e eliminar mensagens de e-mail na sua organização" para obter mais informações.

**Ressarte ou substitua uma mensagem de e-mail que enviou**

1. No painel de pastas à esquerda da janela de Outlook, selecionar a pasta Itens Enviados.
2. Abra a mensagem que pretende ressartar. Tem de fazer duplo clique para abrir a mensagem. Selecionar a mensagem para que seja exibida no painel de leitura não lhe permitirá ressartar a mensagem.
3. No separador Mensagem, selecione **Ações**  >  **Ressartar Esta Mensagem**.
4. **Selecione Eliminar as cópias não** lidas desta mensagem ou Eliminar as cópias não lidas e substituí-as por uma nova mensagem e, em seguida, selecione  **OK.**
5. Se estiver a enviar uma mensagem de substituição, componha a mensagem e, em seguida, selecione **Enviar**.
6. O sucesso ou a falha do ressarcesso de uma mensagem depende das definições dos destinatários Outlook.

Para obter mais informações, incluindo como verificar o ressarto, consulte Ressartar ou [substituir uma mensagem de e-mail que tenha enviado.](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)

***Para procurar e eliminar mensagens de*** e-mail na sua organização , é mais fácil se for um administrador global. Se não for um administrador global, a sua conta tem de ser adicionada ao grupo de funções do Gestor da Deteção de Dados Técnicos ou à função de gestão da Pesquisa de Conformidade. Para eliminar mensagens, terá de aderir ao grupo de funções Gestão da Organização ou à função de Gestão de Pesquisa e Remoção. As permissões para estas funções são atribuídas no [Centro de conformidade & segurança.](https://protection.office.com/)

1. [Crie uma pesquisa de](https://docs.microsoft.com/microsoft-365/compliance/content-search) conteúdo para encontrar a mensagem a eliminar.
2. [Ligação ao PowerShell do & de Conformidade e Segurança.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell)

Se estiver a utilizar MFA (autenticação multifatores), consulte o Ligação para Microsoft 365 PowerShell do Centro de Conformidade & utilizando a autenticação [multifatores.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
