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
ms.openlocfilehash: dfd77bc83b4b278e3630858f54fdfb109ade2a14
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813879"
---
# <a name="encryption-with-transport-rules"></a>Encriptação com regras de transporte

No [Centro de Administração do Exchange](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC), pode utilizar as capacidades de Encriptação de Mensagens do Office (OME) nas suas regras de fluxo de correio para ativar a encriptação de mensagens. Selecione a opção **Aplicar Encriptação de Mensagens e proteção de direitos do Office 365** na condição Regra de Transporte.

- Para mais informações, consulte [Definir regra de fluxo de Correio para encriptar](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

- Na Powershell, use o cmdlet [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) e defina o parâmetro *ApplyOME* como $true.
