---
title: Problemas de sessão nas aplicações da Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2560"
ms.openlocfilehash: 7d2cfd437bb55804c3b9263428833c10d5caaa47
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695334"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Fixação das aplicações Microsoft 365 "Desculpe, outra conta da sua organização já está assinada" mensagem

Para corrigir este erro, experimente o seguinte:

- Remova todas as contas de trabalho, exceto a conta afetada, utilizando as Definições do Windows > **o access ou a escola**.
- [Credenciais de Escritório Claro](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) usando Gestor credencial do Windows.<br/>
    **Nota:** Os percursos de registo do Office 2016 mudaram para 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identidade\)
- Abra uma aplicação **File**do Office, escolha  >  **Account**  >  **'Registar's'.** Em seguida, inscreva-se usando uma conta de utilizador com uma licença válida. Para obter informações detalhadas, consulte [Contas no Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Para Mac, consulte [Não consigo iniciar sessão numa aplicação do Office 2016 para Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Para mais informações, consulte ["Desculpe, outra conta da sua organização já está inscrita neste computador" no Office.](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)