---
title: Os seus utilizadores receberam e-mail malicioso
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 2197e7f195d789193798b80cb092d8046eb6e0be
ms.sourcegitcommit: 3c708a4a349b60b59bc623c44fb78674c685f3c2
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/18/2021
ms.locfileid: "50291803"
---
# <a name="did-your-users-receive-malicious-email"></a>Os seus utilizadores receberam e-mail malicioso?

- Agora pode comunicar o e-mail malicioso à Microsoft através das [submissões de administrador no Centro de Conformidade e Segurança](https://sip.protection.office.com/reportsubmission).

As mensagens que são enviadas nas [submissões de administrador](https://sip.protection.office.com/reportsubmission) são digitalizadas e os seguintes resultados são apresentados na lista de opções de **detalhes**:

- Caso tenha ocorrido uma falha na autenticação de e-mail do remetente no momento da entrega.
- Informações sobre quaisquer ocorrências de política que possam ter afetado ou substituído o veredito de uma mensagem.
- Resultados da detonação atual para ver se os URLs ou os ficheiros contidos na mensagem eram mal-intencionados ou não.
- Feedback das suas notas

Se tiver sido encontrada uma substituição, a nova análise deve ser concluída em vários minutos. Se não existir um problema na autenticação de e-mail ou se a entrega não tiver sido afetada por uma substituição, o feedback das suas notas poderá demorar até um dia.

Se discordar do veredito final de uma mensagem, URL ou ficheiro (bloqueado vs. não bloqueado), envie a mensagem novamente após um dia para digitalizar novamente. Existe uma elevada probabilidade de o veredito ser alterado após submeter a mensagem novamente.

Entretanto, pode remover o e-mail malicioso das caixas de entrada dos utilizadores, seguindo as instruções descritas [neste artigo](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).

- Os clientes com o Microsoft Defender para Office 365 podem:
    - utilizar [o explorador de ameaças para localizar e eliminar e-mails suspeitos](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)
    - [utilizar ligações seguras para bloquear o acesso](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) a um URL malicioso
    - monitorizar os utilizadores que clicarem e acederem a URLs maliciosos: [ver o URL de phishing e clicar em veredito de dados](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)
    - iniciar [manualmente uma investigação automatizada](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)

Também se pode proteger contra ficheiros e URLs maliciosos seguindo as instruções em [Proteção de URLs e ficheiros maliciosos](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).