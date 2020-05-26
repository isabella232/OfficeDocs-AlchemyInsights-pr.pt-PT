---
title: Mensagem de boas-vindas nos Grupos Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "5685"
ms.openlocfilehash: d82931ae6978a09e674b00640d1dd413bcce7cfd
ms.sourcegitcommit: b196100759b29aecd62b693a2bfedbbd25a697c6
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/19/2020
ms.locfileid: "44357837"
---
# <a name="welcome-message-in-microsoft-365-groups"></a>Mensagem de boas-vindas nos Grupos Microsoft 365

Os novos utilizadores que aderirem ao grupo Microsoft 365 receberão um e-mail bem-vindo se a propriedade "UnifiedGroupWelcomeMessageEnabled" for True.

Caso pretenda desativar a mensagem de boas-vindas, utilize o seguinte comando [EXO PowerShell:](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps)

`
Set-UnifiedGroup <groupname> -UnifiedGroupWelcomeMessageEnabled:$False
`
