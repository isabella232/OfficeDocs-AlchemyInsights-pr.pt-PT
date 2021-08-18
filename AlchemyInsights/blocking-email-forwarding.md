---
title: Bloquear ou desbloquear o re encaminhamento de e-mail automático externo
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: fe9e52023b809b38c43332a10a1184d114798cfe
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58315885"
---
# <a name="block-or-unblock-eternal-automatic-email-forwarding"></a>Bloquear ou desbloquear o re encaminhamento automático de e-mails automático desbloqueado

Para ativar ou desativar o re encaminhamento de e-mail para uma caixa de correio específica, consulte [Configurar o re encaminhamento de e-mail.](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)

Os administradores podem controlar o re encaminhamento externo da organização através de políticas de [spam de saída.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy) Pode gerir as políticas de spam de saída no portal do Microsoft 365 Defender em ou através do <https://security.microsoft.com/antispam> cmdlet [Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy) no Exchange Online PowerShell.

Se receber a seguinte mensagem de erro: **"550 5.7.520 O Access foi negado,** a sua organização não permite o re encaminhamento externo", certifique-se de que a política está configurada para ativar as mensagens encaminhadas automaticamente externas.

**Nota:** Recomendamos o valor predefinido Automático **–** o sistema controlado para a definição Regras de re encaminhamento automático na sua política de filtro de spam predefinida (o re encaminhamento externo automático está bloqueado; o encaminhamento automático interno ainda funciona).  Deve criar políticas personalizadas de filtro de spam de saída e utilizar o valor Ativado **-** O re encaminhamento só está ativado para utilizadores que precisem de re encaminhamento de e-mail automático externo. Para obter mais informações, consulte [Configurar o re encaminhamento de e-mail externo Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).
