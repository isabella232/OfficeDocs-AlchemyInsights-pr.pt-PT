---
title: Corrigir problemas de entrega de e-mails em pastas públicas com correio ativado
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: ff1400f694ae037a8658356af068b4c20b8fa9d9908dafedb90db7bb6859530f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54068823"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Corrigir problemas de entrega de e-mails em pastas públicas com correio ativado

Se os remetidos externos não conseguirem enviar mensagens para as suas pastas públicas com correio ativado e os remetidos receberem o erro: não foi possível encontrar **(550 5.4.1),** verifique se o domínio de e-mail da pasta pública está configurado como um domínio de reencaminhamento interno em vez de um domínio autoritativo:

1. Abra o [Exchange de administração do YAC.](https://docs.microsoft.com/Exchange/exchange-admin-center)

2. Aceda **a Fluxo de correio** \> **Domínios aceites**, selecione o domínio aceite e, em seguida, clique em **Editar**.

3. Na página de propriedades que é aberta, se o tipo de domínio estiver definido como **Autoritativo,** altere o valor para **Relay** interno e, em seguida, clique em **Guardar.**

Se os remissões externos receberem a mensagem de erro de que não tem permissão **(550 5.7.13),** execute o seguinte comando no [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) para ver as permissões para utilizadores anónimos na pasta pública:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Por exemplo, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .

Para permitir que os utilizadores externos enviem e-mails para esta pasta pública, adicione o acesso CreateItems ao utilizador Anónimo. Por exemplo, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` .
