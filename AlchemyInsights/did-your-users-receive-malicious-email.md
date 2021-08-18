---
title: Os seus utilizadores receberam e-mail malicioso
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
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: 525af0b29ffa291ddf69f6f2d97f505e93342989
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326715"
---
# <a name="did-your-users-receive-malicious-email"></a>Os seus utilizadores receberam e-mail malicioso?

Agora pode denunciar um e-mail malicioso à Microsoft através [das Submissões no Microsoft 365 Defender portal](https://sip.security.microsoft.com/reportsubmission?viewid=admin).

As mensagens submetidas [em submissões](https://security.microsoft.com/reportsubmission?viewid=admin) de administrador são analisadas e os seguintes resultados apresentados na lista de detalhes:

- Caso tenha ocorrido uma falha na autenticação de e-mail do remetente no momento da entrega.
- Informações sobre quaisquer ocorrências de política que possam ter afetado ou substituído o veredito de uma mensagem.
- Resultados da detonação atual para ver se os URLs ou os ficheiros contidos na mensagem eram mal-intencionados ou não.
- Feedback das suas notas

Se tiver sido encontrada uma substituição, a nova análise deve ser concluída em vários minutos. Se não existir um problema na autenticação de e-mail ou se a entrega não tiver sido afetada por uma substituição, o feedback das suas notas poderá demorar até um dia.

Se discordar do veredito final de uma mensagem, URL ou ficheiro (bloqueado vs. não bloqueado), envie a mensagem novamente após um dia para digitalizar novamente. Existe uma elevada probabilidade de o veredito ser alterado após submeter a mensagem novamente.

Entretanto, pode remover o e-mail malicioso das caixas de entrada dos utilizadores, seguindo as instruções descritas [neste artigo](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).

- Os clientes com o Microsoft Defender para Office 365 podem:
  - Utilizar [o Explorador de Ameaças para Encontrar e Eliminar E-mails Suspeitos](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)
  - [Utilizar Cofre ligações para bloquear o acesso](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-links) a um URL malicioso
  - Controlar utilizadores que clicam e acederam a URLs maliciosos: Ver o URL de [phishing](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer)e clicar em dados de veredito  &  [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)
  - Iniciar [manualmente uma Investigação Automática](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)

Também se pode proteger contra ficheiros e URLs maliciosos seguindo as instruções em [Proteção de URLs e ficheiros maliciosos](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).
