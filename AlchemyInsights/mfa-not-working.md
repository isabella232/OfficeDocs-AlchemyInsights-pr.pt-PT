---
title: Problemas com o MFA
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 718af9bfbc0a64cdfc96528e5062fb96c8d0f2d3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47755142"
---
# <a name="issues-with-azure-mfa"></a>Problemas com Azure MFA
Há algumas coisas para verificar se os utilizadores não podem iniciar sessão usando a autenticação de vários fatores (MFA)

1. O utilizador afetado pode estar bloqueado no Portal do Diretório Ativo Azure. Se for esse o caso, as tentativas de autenticação para esse utilizador específico serão automaticamente negadas. [Por favor, siga os passos deste artigo para desbloqueá-los.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Se desbloquear o utilizador não ajudou ou o utilizador não está bloqueado, pode tentar reiniciar o MFA para o utilizador e passará novamente pelo processo de inscrição. [Por favor, siga os passos deste artigo.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Se esta for a primeira vez que ativou o MFA e os seus utilizadores não puderem iniciar sessão em clientes não-navegadores como o Outlook, Skype, etc, talvez a ADAL (Ative Directory Authentication Library) não esteja ativada na sua subscrição O365. Neste caso, você precisará ligar-se ao Exchange Online Powershell e executar este cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*