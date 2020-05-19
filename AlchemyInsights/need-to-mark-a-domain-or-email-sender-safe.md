---
title: Precisa marcar um domínio ou e-mail cofre?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 7dc1576fd61e87b319c7486c59ed125943b4d959
ms.sourcegitcommit: 43acdecef129bfffc8bbe8ebb08fdd581b238a03
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/18/2020
ms.locfileid: "44281182"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Precisa marcar um domínio ou e-mail cofre?

- A utilização de listas de **remetentes seguras não é recomendada,** uma vez que abre a sua organização a ataques de spam, phish e falsificação.
- No entanto, se houver um requisito de negócio, **recomendamos** a utilização de Regras de Fluxo de **[Correio](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** para o mesmo. A nossa orientação garante a autenticação do remetente (verifica que o domínio de envio não está a ser falsificado). **Nota:** Não recomendamos gerir falsos positivos utilizando listas de remetentes seguras, porque exceções à filtragem de spam podem abrir a sua organização a ataques de segurança. Se o seu utilizador(s) receber mensagens incorretamente marcadas como correio publicitário não solicitado ou lixo, por **[favor, informe mensagens e ficheiros para a Microsoft](https://protection.office.com/reportsubmission)**.
- Os remetentes seguros no Outlook, a lista de remetentes permitidas ou a lista de domínios permitidas nas políticas anti-correio publicitário não solicitado **devem ser evitadas** porque os remetentes contornam todos os spam, spoof e phish protection, e a autenticação do remetente (SPF, DKIM, DMARC). Este método é melhor utilizado apenas para testes temporários.
