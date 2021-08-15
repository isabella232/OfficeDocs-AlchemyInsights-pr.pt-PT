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
ms.openlocfilehash: b134c952e3cc5305d8f3e6f44031e7f33d7938b67ff122c46cb74bbd33cbf59e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53994876"
---
# <a name="set-clientaccessserverenabled-to-true"></a>Definir ClientAccessServerEnabled para True

Se não conseguir abrir uma mensagem de e-mail encriptado e, em vez disso, vir um **anexo rpmsg,** execute os seguintes passos:

1. Ligação para Exchange Online PowerShell.

> [!NOTE]
> Para se ligar a Exchange Online PowerShell, tem de entrar com um administrador global ou Exchange de administrador.

   a. Abra Windows PowerShell e, em seguida, execute o seguinte comando:`$UserCredential = Get-Credential`
b. Na caixa **de Windows PowerShell Pedido de Credencial,** introduza a sua conta escolar ou escolar e a sua palavra-passe, c. Clique em **OK**. 

2. Execute o seguinte comando para criar uma nova sessão:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. Execute o seguinte comando:
    
    `Import-PSSession $Session -DisableNameChecking`

3. Comando `Get-IRMConfiguration` Executar.

4. Verifique **a definição ClientAccessServerEnabled.** 

    a. Se **a definição ClientAccessServerEnabled** estiver definida como **False,** execute o seguinte cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

> [!TIP]
> Feche sempre a sua sessão do PowerShell com o seguinte comando: `Remove-PSSession $Session`

Para obter mais informações, [consulte Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

