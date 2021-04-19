---
title: Resolução de problemas de autenticação SMTP
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
- "3000003"
- "5652"
ms.openlocfilehash: 2d3f0f6b700c3e4485c9064fbaa4bcc165e92e17
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826426"
---
# <a name="solving-smtp-authentication-issues"></a>Resolução de problemas de autenticação SMTP

Se estiver a obter erros 5.7.57 ou 5.7.3 ao tentar enviar e-mail SMTP e autenticar com um cliente ou aplicação, há algumas coisas que deve verificar:

- A submissão autenticada do SMTP pode ser desativada no seu inquilino ou na caixa de correio que está a tentar utilizar (verifique ambas as definições). Para ler mais, consulte [Ativar ou desativar a submissão do cliente autenticado SMTP](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).

- Verifique se [os Incumprimentos de Segurança Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) estão ativados para o seu inquilino; se ativado, a autenticação SMTP utilizando a autenticação básica (também conhecida como legado; isto utilizará o nome de utilizador e a palavra-passe) falhará.
