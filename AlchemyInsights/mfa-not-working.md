---
title: Problemas com mfa
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
ms.openlocfilehash: a415116b9ba437cb13426896119cd1b40d9ab491
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/15/2019
ms.locfileid: "37768848"
---
# <a name="issues-with-azure-mfa"></a>Problemas com o Azure MFA
Há algumas coisas para verificar se os usuários não podem fazer login usando autenticação multifator (MFA)

1. O usuário afetado pode ser bloqueado no Portal de Diretório Ativo do Azure. Se for esse o caso, as tentativas de autenticação para esse usuário específico serão automaticamente negadas. [Por favor, siga os passos deste artigo para desbloqueá-los.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Se desbloquear o usuário não ajudou ou o usuário não estiver bloqueado, você pode tentar redefinir o MFA para o usuário e eles passarão pelo processo de inscrição novamente. [Por favor, siga os passos deste artigo.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Se esta for a primeira vez que você habilitado MFA e seus usuários são incapazes de fazer login em clientes não-navegadores, como Outlook, Skype, etc, talvez ADAL (Active Directory Authentication Library) não está habilitado em sua assinatura O365. Neste caso, você precisará se conectar à Troca online powershell e executar este cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*