---
title: Utilize o Exchange Online PowerShell para permitir ao DKIM um domínio específico
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
ms.openlocfilehash: 2f2b60a63b512bde794ba588852db11423e766f3
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749727"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>Utilize o Exchange Online PowerShell para permitir ao DKIM um domínio específico

Se não conseguir criar os registos DKIM DNS no centro de administração, tente utilizar o Exchange Online PowerShell. 

Para criar um registo DKIM DNS utilizando o Exchange Online PowerShell, execute os seguintes passos:

1. Abra o Windows PowerShell como administrador e execute os seguintes comandos na sequência descrita:

    a. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c. `Import-PSSession $Session -DisableNameChecking`
    
Se tiver problemas em ligar-se ao Exchange Online PowerShell, consulte [Connect to Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).

2. Uma vez ligado ao Exchange Online PowerShell, execute o seguinte comando:

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. Uma vez executado com sucesso o comando acima, execute o seguinte comando para encerrar a sessão Exchange Online PowerShell:

    `Remove-PSSession $Session` 



