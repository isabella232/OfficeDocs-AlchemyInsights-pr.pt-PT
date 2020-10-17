---
title: 726 Encaminhamento de e-mail de bloqueio
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
ms.openlocfilehash: 610013c4f46e999f1a8715aea14dd557ed8b0e2a
ms.sourcegitcommit: 88f24bb6ced16842de165af416e3f21feae13063
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/15/2020
ms.locfileid: "48478341"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>Bloquear ou desbloquear o reencaminhamento de e-mails

Para ativar ou desativar o reencaminhamento de e-mails para uma caixa de correio específica, consulte o [reencaminhamento de e-mail Configure](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

Ao nível dos inquilinos, o controlo do encaminhamento externo é feito utilizando a política de spam de saída. Pode consultar a política de filtro de spam de saída do Centro de Segurança e Conformidade [aqui](https://protection.office.com/antispam) ou utilizando o [comando Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).

Se estiver a obter o seguinte erro: **"550 5.7.520 Acesso negado, a sua organização não permite o encaminhamento externo"**, certifique-se de que a política está configurada para ativar o Auto-forward Externo.

**Nota:** Recomenda-se manter o Autoforward Externo desativado na sua política de filtro de spam por defeito e permitir apenas para os utilizadores que necessitem de reencaminhamento externo, criando uma política personalizada para esses utilizadores. Pode ler mais na [configuração do reencaminhamento de e-mails externos no Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).