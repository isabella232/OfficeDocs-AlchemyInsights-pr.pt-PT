---
title: Corrigir problemas de entrega de e-mail para pastas públicas via correio
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: e261fe60843555fa45927b0a6b36e1ccf79fb028
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716363"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Corrigir problemas de entrega de e-mail para pastas públicas via correio

Se os remetentes externos não puderem enviar mensagens para as suas pastas públicas ativadas por correio, e os remetentes receberem o erro: **não puderam ser encontrados (550 5.4.1),** verifique se o domínio de e-mail da pasta pública está configurado como um domínio interno de retransmissão em vez de um domínio autoritário:

1. Abra o centro de [administração exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Vá ao **fluxo** \> de correio **Domínios aceitos,** selecione o domínio aceite e, em seguida, clique em **Editar**.

3. Na página de propriedades que se abre, se o tipo de domínio for definido para **Authoritativo,** altere o valor para **retransmissão interna** e, em seguida, clique em **Guardar**.

Se os remetentes externos receberem o erro, **não tem permissão (550 5.7.13)**, executar o seguinte comando no [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) para ver as permissões para utilizadores anónimos na pasta pública:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Por exemplo, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.

Para permitir que utilizadores externos enviem e-mail para esta pasta pública, adicione o acesso do CreateItems ao utilizador Anónimo. Por exemplo, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.
