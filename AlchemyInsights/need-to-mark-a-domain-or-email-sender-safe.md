---
title: Precisa marcar um domínio ou cofre de remetente de e-mail?
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
- "9002921"
- "5673"
ms.openlocfilehash: 0ea089b95ad7de25e77017196fb2db895d4d0178
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47803256"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Precisa marcar um domínio ou cofre de remetente de e-mail?

- A utilização de **listas de remetentes seguras não é recomendada,** uma vez que abre a sua organização para spam, phish e falsificação de ataques.
- No entanto, se houver um requisito de negócio, **recomendamos** a utilização **[de Regras de Fluxo de Correio](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** para isso. A nossa orientação garante a autenticação do remetente (verifica-se que o domínio de envio não está a ser falsificado). **Nota:** Não recomendamos a gestão de falsos positivos utilizando listas de remetentes seguras, porque exceções à filtragem de spam podem abrir a sua organização a ataques de segurança. Se o seu(s) utilizador(s) receber mensagens incorretamente marcadas como correio publicitário não solicitado ou correio eletrónico de sucata, por favor **[reporte mensagens e ficheiros à Microsoft](https://protection.office.com/reportsubmission)**.
- Os Remetentes Seguros no Outlook, a lista de remetentes permitidos ou a lista de domínios permitida nas políticas anti-correio publicitário não-correio **publicitário não-correio eletrónico devem ser evitados** porque os remetentes contornam toda a proteção de spam, spoof e phish e a autenticação do remetente (SPF, DKIM, DMARC). Este método é melhor utilizado apenas para testes temporários.
