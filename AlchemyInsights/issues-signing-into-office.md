---
title: Problemas de sessão em apps do Office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2574"
ms.openlocfilehash: 695d449a876c22ff441da2367ef67aaea470eb66
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43763012"
---
# <a name="issues-signing-in-to-office-apps"></a>Problemas de sessão em apps do Office

Para corrigir problemas de inscrição com aplicações do Office, tente o seguinte:

- Remova todas as contas de trabalho, exceto a conta afetada, utilizando as definições do Windows > **Trabalho de Acesso ou escola**.
- [Credenciais de escritório claro](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) usando O Gestor Credencial do Windows.<br/>
    **Nota:** As vias de registo do Office 2016 mudaram para 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Abra uma aplicação do Office, **escolha** > **Registo de Conta** > **Sign out**. Em seguida, inscreva-se utilizando uma conta de utilizador com uma licença válida. Para obter informações detalhadas, consulte [Contas no Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Para Mac, consulte [Não consigo iniciar sessão numa aplicação do Office 2016 para Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).
- Se os erros ocorrerem durante a ligação ao Microsoft 365 utilizando o Office 2013, ative a autenticação moderna para o cliente do Office.

Para obter mais informações, consulte:
- [Não pode iniciar sessão na Microsoft 365, Azure ou Intune](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [Problemas de ligação no registo após atualização para o Office 2016 constroem 16.0.7967 no Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- ["Desculpe, outra conta da sua organização já está assinada neste computador" no Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [Problemas de sessão de sessão com autenticação moderna do Office quando utiliza a ADFS](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)