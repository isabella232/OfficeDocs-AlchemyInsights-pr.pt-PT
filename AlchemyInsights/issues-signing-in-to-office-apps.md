---
title: Problemas ao inscrever-se Microsoft 365 aplicações
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2560"
ms.openlocfilehash: 454000eafa6818f91e3c302cc69fbf252aae1107aa18904ac93a4756d4db642b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028051"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Corrigir a mensagem Microsoft 365 aplicações "Lamentamos, mas já tem a mesma conta da sua organização"

Para corrigir este erro, experimente o seguinte:

- Remova todas as contas de trabalho, exceto a conta afetada, Windows Definições > **escolar ou escolar do Access.**
- [Limpe Office de credenciais utilizando](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) o Windows de Credenciais.<br/>
    **Nota:** Os caminhos de registo Office 2016 mudaram para 16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Abra um aplicação do Office, selecionar **Saída**  >  **de Conta** de  >  **Ficheiro**. Em seguida, inscreva-se com uma conta de utilizador com uma licença válida. Para obter informações detalhadas, consulte [Contas no Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Para Mac, consulte [Não consigo iniciar sessão numa aplicação do Office 2016 para Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Para obter mais informações, consulte ["Lamentamos,](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)mas já tem a sua conta com a sua organização com a sua conta neste computador" no Office .