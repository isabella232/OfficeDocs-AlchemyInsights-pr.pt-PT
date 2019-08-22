---
title: Converter caixa de correio do utilizador para uma caixa de correio partilhada?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Normal
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: ab34b8939b95b29bedb797f640dd744bc783adef
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36496446"
---
# <a name="convert-a-user-mail-box-into-a-shared-mailbox"></a>Converter uma caixa de correio do utilizador uma caixa de correio partilhada

Só pode converter uma caixa de correio do utilizador para uma caixa de correio partilhada, se o utilizador tiver uma licença de Exchange. Depois da caixa de correio é convertida, continuará a aparecer na lista de utilizadores do active uma vez que essa lista inclui caixas de correio partilhadas. No entanto, a caixa de correio convertida também aparecerá na lista de caixa de correio partilhada. 
  
Se tentar converter uma caixa de correio na consola de administração do Exchange e a conversão falha, limpar a cache do browser e os cookies e tente novamente. Se ainda não funcionar, tente converter a caixa de correio no Exchange Management Shell executando o seguinte comando:
  
```
Set-Mailbox -Type Shared
```

Mais informações de conversão de caixa de correio estão disponíveis no [converter uma caixa de correio do utilizador para uma caixa de correio partilhada](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).
  
