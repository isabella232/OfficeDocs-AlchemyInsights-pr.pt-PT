---
title: Problemas com MFA
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 276f6b2212c9d85df726cb46a46dee7828b34c89
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/18/2019
ms.locfileid: "36545187"
---
# <a name="issues-with-mfa"></a>Problemas com MFA
Há algumas coisas para verificar se os usuários não podem fazer login usando a autenticação multifator (MFA)

1. O usuário afetado pode ser bloqueado no portal do Active Directory do Azure. Se for esse o caso, as tentativas de autenticação para esse usuário específico serão negadas automaticamente. [Por favor, siga os passos neste artigo para desbloqueá-los.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Se o desbloqueio do usuário não ajudar ou o usuário não estiver bloqueado, você poderá tentar redefinir a MFA para o usuário e eles irão passar pelo processo de registro novamente. [Por favor, siga os passos neste artigo.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Se esta for a primeira vez que você habilitou o MFA e seus usuários não conseguem fazer logon em clientes que não sejam navegadores, como Outlook, Skype, etc, talvez a ADAL (biblioteca de autenticação do Active Directory) não esteja habilitada na sua assinatura do O365. Nesse caso, será necessário conectar-se ao PowerShell do Exchange Online e executar este cmdlet:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*