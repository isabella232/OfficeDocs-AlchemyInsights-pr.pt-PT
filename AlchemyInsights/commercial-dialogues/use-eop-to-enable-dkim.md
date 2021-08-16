---
title: Utilizar Exchange Online PowerShell para ativar o DKIM para um domínio específico
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: ba627c6da96624914b858aa09d6eff9de709134c2c986fe363845c5ab2b66434
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54070322"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>Utilizar Exchange Online PowerShell para ativar o DKIM para um domínio específico

Se não conseguir criar os registos DKIM DNS no centro de administração, experimente utilizar o Exchange Online PowerShell. 

Para criar um registo DKIM DNS com o Exchange Online PowerShell, execute os seguintes passos:

1. Abra Windows PowerShell como administrador e execute os seguintes comandos na sequência descrita:

    a. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c. `Import-PSSession $Session -DisableNameChecking`
    
Se tiver problemas a ligar ao Exchange Online PowerShell, [consulte Ligação o Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

2. Assim que estiver ligado ao Exchange Online PowerShell, execute o seguinte comando:

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. Assim que o comando acima tiver sido executado com êxito, execute o seguinte comando para terminar a Exchange Online sessão do PowerShell:

    `Remove-PSSession $Session` 



