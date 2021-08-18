---
title: Definir ClientAccessServerEnabled para True
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: fc953813a94c9ed3226f81f776d6085e12a6cafc
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320367"
---
# <a name="set-clientaccessserverenabled-to-true"></a>Definir ClientAccessServerEnabled para True

Se não conseguir abrir uma mensagem de e-mail encriptado e, em vez disso, vir um **anexo rpmsg,** execute os seguintes passos:

1. Ligação a Exchange Online PowerShell.

    **Nota:** para se ligar a Exchange Online PowerShell, tem de entrar com um administrador global ou uma Exchange de administração.

   a. Abra Windows PowerShell e, em seguida, execute o seguinte comando:`$UserCredential = Get-Credential`
   b. Na caixa **Windows PowerShell Pedido de Credencial,** introduza a sua conta escolar ou escolar e a sua palavra-passe, c. Clique em **OK**. 

2. Execute o seguinte comando para criar uma nova sessão:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. Execute o seguinte comando:
    
    `Import-PSSession $Session -DisableNameChecking`

3. Comando `Get-IRMConfiguration` Executar.

4. Verifique **a definição ClientAccessServerEnabled.** 

    a. Se **a definição ClientAccessServerEnabled** estiver definida como **False,** execute o seguinte cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

**Sugestão:** feche sempre a sua sessão do PowerShell com o seguinte comando: `Remove-PSSession $Session`

Para obter mais informações, [consulte Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

