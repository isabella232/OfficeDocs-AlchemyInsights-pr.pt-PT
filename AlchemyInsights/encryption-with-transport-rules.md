---
title: Encriptação com regras de transporte
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5154"
ms.openlocfilehash: e1f8227047daede71d0fa3b3557db0d95a379b99b76ab0c2fe1d6ed8cc213d4a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54079461"
---
# <a name="encryption-with-transport-rules"></a>Encriptação com regras de transporte

No [Centro de Administração do Exchange](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC), pode utilizar as capacidades de Encriptação de Mensagens do Office (OME) nas suas regras de fluxo de correio para ativar a encriptação de mensagens. Selecione a opção **Aplicar Encriptação de Mensagens e proteção de direitos do Office 365** na condição Regra de Transporte.

- Para mais informações, consulte [Definir regra de fluxo de Correio para encriptar](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

- Na Powershell, use o cmdlet [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) e defina o parâmetro *ApplyOME* como $true.
