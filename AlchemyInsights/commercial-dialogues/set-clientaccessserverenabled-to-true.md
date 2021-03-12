---
title: Definir ClienteAccessServerEnabled a True
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
ms.openlocfilehash: 2adf35662797e9e9e354ddd0c513f5ce2463d07c
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749980"
---
# <a name="set-clientaccessserverenabled-to-true"></a>Definir ClienteAccessServerEnabled a True

Se não conseguir abrir uma mensagem de correio eletrónico encriptada e, em vez disso, ver um anexo **rpmsg,** execute os seguintes passos:

1. Ligue-se a Exchange Online PowerShell.

> [!NOTE]
> Para se ligar ao Exchange Online PowerShell, tem de iniciar scontabilidade através de uma conta de administração global ou de administração Exchange.

   a. Abra o Windows PowerShell e, em seguida, execute o seguinte comando: `$UserCredential = Get-Credential`
b. Na caixa de diálogo **de pedido de pedido de procura do Windows PowerShell,** insira a sua conta de trabalho ou escola e a palavra-passe, c. Clique em **OK**. 

2. Executar o seguinte comando para criar uma nova sessão:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. Run the following command:
    
    `Import-PSSession $Session -DisableNameChecking`

3. Executar `Get-IRMConfiguration` o comando.

4. Verifique a definição **ClientAccessServerEnabled.** 

    a. Se a definição **DeServerEnabled do Cliente** estiver definida como **Falsa,** executar o seguinte cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

> [!TIP]
> Feche sempre a sua sessão de powershell com o seguinte comando: `Remove-PSSession $Session`

Para mais informações, consulte [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).

