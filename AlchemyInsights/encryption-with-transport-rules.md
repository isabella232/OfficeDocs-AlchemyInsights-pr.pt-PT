---
title: Encriptação com regras de transporte
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5154"
ms.openlocfilehash: 3f16c7e7be99a50cd57f47ea2801b3022c4aec95
ms.sourcegitcommit: 07725fcaf073f0ac145f98653b989afdb34c5ad0
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/28/2020
ms.locfileid: "43915169"
---
# <a name="encryption-with-transport-rules"></a>Encriptação com regras de transporte

No [Centro de Administração do Exchange](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC), pode utilizar as capacidades de Encriptação de Mensagens do Office (OME) nas suas regras de fluxo de correio para ativar a encriptação de mensagens. Selecione a opção **Aplicar Encriptação de Mensagens e proteção de direitos do Office 365** na condição Regra de Transporte.

- Para mais informações, consulte [Definir regra de fluxo de Correio para encriptar](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

- Na Powershell, use o cmdlet [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) e defina o parâmetro *ApplyOME* como $true.
