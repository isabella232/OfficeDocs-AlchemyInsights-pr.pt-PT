---
title: Erro de endereço proxy ao criar uma caixa de correio partilhada
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
ms.openlocfilehash: 7c15d5db5445fbe4c3ec22878f180f48d2da4f90369f2e6f223916646eb19c12
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54062919"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a>Erro de endereço proxy ao criar uma caixa de correio ou outro objeto com e-mail ativado

Se tentou criar um objeto com capacidade de e-mail (caixa de correio, caixa de correio partilhada, etc.) e recebeu o erro "O endereço proxy "O endereço proxy "SMTP:alias@domain.com" já está a ser utilizado...", o endereço de e-mail que escolheu já é retirado por outro objeto com capacidade de e-mail na sua organização.
  
Tem de encontrar o utilizador, grupo, caixa de correio partilhada ou pasta pública que tem este endereço de e-mail e eliminá-lo ou alterar o respetivo endereço de e-mail. Em seguida, pode criar um novo objeto com e-mail com o endereço de e-mail libertado. Utilize a pesquisa na Home page para encontrá-la. Também pode utilizar o seguinte comando Exchange Online PowerShell para procurá-lo:

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
Se não quiser eliminar o endereço de e-mail existente, escolha um novo endereço de e-mail para o novo objeto que está a criar.
  