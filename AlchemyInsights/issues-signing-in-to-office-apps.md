---
title: Problemas de sessão nas aplicações da Microsoft 365
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
ms.openlocfilehash: 8065a49c42953013ccfae9c5c1714d10ee0b4d49
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833086"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Fixação das aplicações Microsoft 365 "Desculpe, outra conta da sua organização já está assinada" mensagem

Para corrigir este erro, experimente o seguinte:

- Remova todas as contas de trabalho, exceto a conta afetada, utilizando as Definições do Windows > **o access ou a escola**.
- [Credenciais de Escritório Claro](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) usando Gestor credencial do Windows.<br/>
    **Nota:** Os percursos de registo do Office 2016 mudaram para 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identidade\)
- Abra uma aplicação do Office, escolha  >    >  **'Registar's'.** Em seguida, inscreva-se usando uma conta de utilizador com uma licença válida. Para obter informações detalhadas, consulte [Contas no Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Para Mac, consulte [Não consigo iniciar sessão numa aplicação do Office 2016 para Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Para mais informações, consulte ["Desculpe, outra conta da sua organização já está inscrita neste computador" no Office.](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)