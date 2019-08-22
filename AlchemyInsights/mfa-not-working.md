---
title: Problemas relacionados com AMF
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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36545187"
---
# <a name="issues-with-mfa"></a>Problemas relacionados com AMF
Existem algumas coisas para verificar se os utilizadores não podem iniciar sessão utilizando autenticação multi-factores (AMF)

1. O utilizador afectado poderão ser bloqueado no Portal de directório Active Azure. Se for esse o caso, tentativas de autenticação para esse utilizador específico será automaticamente recusado. [Siga os passos neste artigo para desbloqueá-los.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Se desbloquear o utilizador ajudou ou o utilizador não está bloqueado pode tentar repor AMF para o utilizador e que aceitem através do processo de inscrição novamente. [Siga os passos descritos neste artigo.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Se esta for a primeira vez AMF activado e os utilizadores não conseguem iniciar sessão para clientes não browsers, tais como o Outlook, Skype, etc, talvez ADAL (Active Directory autenticação biblioteca) não está activada na sua subscrição de O365. Neste caso terá de ligar ao Exchange Online Powershell e executar este cmdlet:  *conjunto-OrganizationConfig-OAuth2ClientProfileEnabled: $true*