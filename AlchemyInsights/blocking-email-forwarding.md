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
ms.openlocfilehash: c0d9ed14f83d3c7d47e1728d5ed9ca3a19412ad2
ms.sourcegitcommit: f74c9698a31634154ce58dda8b3145bb10685ace
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/23/2020
ms.locfileid: "48219866"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>Bloquear ou desbloquear o reencaminhamento de e-mails

Para ativar ou desativar o reencaminhamento de e-mails para uma caixa de correio específica, consulte o [reencaminhamento de e-mail Configure](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

Ao nível dos inquilinos, o controlo do reencaminhamento externo é feito utilizando a política anti-correio publicitário não-correio eletrónico de saída. Se estiver definido para Off ou Automatic, poderá bloquear o reencaminhamento de e-mails com o erro de "Acesso 550 5.7.520 negado, a sua organização não permite o encaminhamento externo". Posteriormente, se o encaminhamento foi definido para ser bloqueado, este é o erro que os seus utilizadores verão.

Se o encaminhamento estiver bloqueado, certifique-se de que a política está configurada para ativar o autoforário externo. Pode consultar a Política de Filtro de Spam de Saída do Centro de Segurança e Conformidade ou executando o comando Get-HostedOutboundSpamFilterPolicy / nome fl,AutoForwardingMode. Se quiser configurar o bloqueio auto-forward, o mesmo comando dir-lhe-á agora o estado da política.

Nota: É aconselhável manter o autoforário externo desativado na sua Política de Filtro de Correio publicitário não solicitado por defeito e permitir que este seja apenas para os utilizadores que necessitem de reencaizá-lo externo, criando uma política personalizada para esses utilizadores. Pode ler mais na [configuração do reencaminhamento de e-mails externos no Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).