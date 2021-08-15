---
title: Precisa de marcar um domínio ou remetente de e-mail em segurança?
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
- "9002921"
- "5673"
ms.openlocfilehash: 7058b6419e52fce94f3359d0bd8e1d67c5aa5ef6743abf4ed39f45bad49e1d07
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54025621"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Precisa de marcar um domínio ou remetente de e-mail em segurança?

- A utilização **de listas** de remetentes seguros não é recomendada, uma vez que abre a sua organização com ataques de spam, phish e spoofing.
- No entanto, se for necessário na empresa, recomendamos **que utilize** as Regras Flow **[Correio para](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** este caso. As nossas orientações garantem que a autenticação do remetente (verifica se o domínio de envio não está a ser spoofed). **Nota:** não recomendamos a gestão de falsos positivos ao utilizar listas de remetente seguras, uma vez que as exceções à filtragem de spam podem abrir a sua organização a ataques de segurança. Se os seus utilizadores receberem mensagens marcadas incorretamente como spam ou e-mail de lixo, reporte mensagens e **[ficheiros à Microsoft.](https://protection.office.com/reportsubmission)**
- Cofre Os remetentes no Outlook, na lista de remetentes permitidos ou na lista de domínios permitidos nas políticas antisspam devem ser evitados porque os remetentes não remetentes desviam todo o spam, spoof, proteção de phish e a autenticação do remetente (SPF, DKIM, DMARC).  Este método é mais adequado para testes temporários apenas.
- A validação de que um determinado **[e-mail](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)** desviado da avaliação Antisspam pode ser efetuada seleindo o cabeçalho da mensagem "X-Forefront-Antispam-Report" (SFV:SFE, SFV:SKA, SFV:SKN), consulte Cabeçalhos de mensagens antisspam.
- Uma vez que a [](https://docs.microsoft.com/microsoft-365/security/office-365-security/secure-by-default#exceptions)Microsoft quer manter os nossos clientes seguros por predefinição, algumas substituições dos inquilinos não são aplicadas a software malware e phishing de alta confiança. Estas substituições incluem: o Listas de remetentes permitidos ou listas de domínios permitidas (políticas antisspam) o Outlook Cofre Remetentes o IP Allow List (filtragem de ligação) 
- A única override que permite que a mensagem de phishing de alta confiança desconfie da filtragem seja Exchange regras de fluxo de correio (também conhecidas como regras de transporte). Para utilizar regras de fluxo de correio para ultrapassar a filtragem, consulte Utilizar regras de fluxo de correio para definir o nível de confiança contra **[spam (SCL) nas mensagens.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-mail-flow-rules-to-set-the-spam-confidence-level-scl-in-messages)**