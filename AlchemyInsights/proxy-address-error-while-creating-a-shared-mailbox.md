---
title: Erro de endereço de procuração ao criar uma caixa de correio partilhada
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: ab491e883ab294f08d0b5d2e686dc059b468d29f
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568301"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a>Erro de endereço de procuração ao criar uma caixa de correio ou outro objeto ativado por e-mail

Se tentou criar um objeto ativado por e-mail (caixa de correio, caixa de correio partilhada, etc.) e recebeu o erro "O endereço de procuração "SMTP:alias@domain.com" já está a ser utilizado...", o endereço de e-mail que escolheu já está a ser tomado por outro objeto habilitado por e-mail na sua organização.
  
Tem de encontrar o utilizador, grupo, caixa de correio partilhada ou pasta pública que tenha este endereço de e-mail e elimine-o ou altere o seu endereço de e-mail. Em seguida, pode criar um novo objeto ativado por e-mail com o endereço de e-mail libertado. Utilize a pesquisa na página inicial para encontrá-la. Também pode utilizar o seguinte comando Exchange Online PowerShell para o procurar:

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
Se não pretender eliminar o endereço de e-mail existente, escolha um novo endereço de e-mail para o novo objeto que está a criar.
  