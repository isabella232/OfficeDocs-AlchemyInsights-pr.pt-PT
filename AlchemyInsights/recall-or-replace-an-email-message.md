---
title: Resgatar ou substituir uma mensagem de correio electrónico
ms.author: daeite
author: daeite
manager: joallard
ms.date: 05/15/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: d5952041f6f2fd736e975abf06cc22880d21a089
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36553443"
---
# <a name="recall-or-replace-an-email-message-in-office-365"></a>Resgatar ou substituir uma mensagem de correio electrónico no Office 365

- Pode **apenas mensagens de recuperação que são enviadas para pessoas na organização**. Se a mensagem foi enviada para um endereço de Gmail, por exemplo, não se lembrá-lo.
- Pode **apenas resgatar as mensagens enviadas de 2016 do Outlook para o PC**. Se um utilizador envia uma mensagem utilizando o Outlook para Mac ou o Outlook na web, não se lembrá-lo.
- Se for um administrador, pode **resgate de mensagens em nome dos utilizadores através do PowerShell**. Não é possível recuperar mensagens a partir do Centro de administração. Desloque-se para "Procurar e eliminar mensagens de correio electrónico da empresa" para obter mais informações.

**Resgatar ou substituir uma mensagem de correio electrónico de envio**

1. No painel de pastas do lado esquerdo da janela do Outlook, seleccione a pasta Itens enviados.
2. Abra a mensagem que pretende recuperar. Deve fazer duplo clique para abrir a mensagem. Seleccionando a mensagem para que apareça no painel de leitura não permite-lhe resgatar a mensagem.
3. Separador mensagem, seleccione **Acções** > **Resgatar a mensagem**.
4. Optar por **Eliminar as cópias não lidas desta mensagem** ou **elimine cópias não lidas e substitua por uma nova mensagem**, em seguida, seleccione **' OK '**.
5. Se estiver a enviar uma mensagem de substituição, compor a mensagem, em seguida, seleccione **Enviar**.
6. O êxito ou falha do resgate de mensagens depende de definições dos destinatários do Outlook.

Para mais informações, incluindo como verificar a recuperação, consulte [resgatar ou substituir uma mensagem de correio electrónico que enviou](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

***Procurar e eliminar mensagens de correio electrónico na organização*** Para procurar e eliminar mensagens de correio electrónico na organização, é mais fácil se for um administrador global. Se não for um administrador global, deve ser adicionada a conta para o grupo de funções de Gestor de detecção de dados electrónicos, ou para a função de gestão da procura de conformidade. Para eliminar mensagens, terá de associar o grupo de funções de gestão da organização ou a função de gestão de procura e remover. Permissões para estas funções são atribuídas no [Centro de conformidade de & de segurança](https://protection.office.com/).

1. [Criar um conteúdo de procura](https://docs.microsoft.com/office365/securitycompliance/content-search) para localizar a mensagem para eliminar.
2. [Estabelecer ligação com segurança & conformidade Centro PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps). 

Se estiver a utilizar AMF, consulte [ligar a & de segurança do Office 365 PowerShell do Centro de conformidade a utilizar a autenticação de factor múltiplos](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps). 
