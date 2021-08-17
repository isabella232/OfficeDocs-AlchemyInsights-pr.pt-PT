---
title: 726 Bloquear o re encaminhamento de e-mail
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
ms.openlocfilehash: 0bff7ede02809e133dc6616452ec840f552bd4fa6c45b7987d6455b2a9ba49bf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059643"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>Bloquear ou desbloquear o recarregamento de e-mails

Para ativar ou desativar o re encaminhamento de e-mail para uma caixa de correio específica, consulte [Configurar o re encaminhamento de e-mail.](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)

Ao nível do inquilino, o controlo do re encaminhamento externo é realizado através da política de spam de saída. Pode consultar a política de filtro de spam [](https://protection.office.com/antispam) de saída a partir do Centro de Conformidade e Segurança aqui ou através do comando [Get-HostedOutboundSpamFilterPolicy.](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy)

Se estiver a obter o seguinte erro: **"550 5.7.520 O Access foi negado,** a sua organização não permite o re encaminhamento externo", certifique-se de que a política está configurada para ativar o Encaminhamento Automático Externo.

**Nota:** Recomendamos que mantenha a ativação automática externa desativada na sua política do filtro de spam de saída predefinida e ative-a apenas para os utilizadores que necessitam de re encaminhamento externo através da criação de uma política personalizada para esses utilizadores. Pode ler mais em Configurar o [re encaminhamento de e-mail externo no Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).