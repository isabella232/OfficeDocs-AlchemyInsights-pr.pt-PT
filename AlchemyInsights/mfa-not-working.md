---
title: Problemas com a MFA
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: b39c79063c66ea41585c8f9eec372bfac77bc0aa29ded5a5572e06c141b28f80
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098613"
---
# <a name="issues-with-azure-mfa"></a>Problemas com o MFA do Azure
Existem alguns aspas a verificar se os utilizadores não conseguem iniciar sessão com a autenticação multifatores (MFA)

1. O utilizador afetado poderá estar bloqueado no Azure Active Directory Portal. Se for esse o caso, as tentativas de autenticação para esse utilizador específico serão negadas automaticamente. [Siga os passos neste artigo para os desbloquear.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Se o desbloqueio não tiver ajudado o utilizador ou se o utilizador não estiver bloqueado, pode tentar repor a MFA do utilizador e esse utilizador irá novamente através do processo de inscrição. [Siga os passos neste artigo.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Se esta for a primeira vez que ativou a MFA e os seus utilizadores não conseguirem fazer login em clientes que não sejam browsers, como o Outlook, Skype, etc. talvez a ADAL (Biblioteca de Autenticação do Active Directory) não esteja ativada na sua subscrição do O365. Neste caso, terá de ligar ao Exchange Online PowerShell e executar este cmdlet: *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*