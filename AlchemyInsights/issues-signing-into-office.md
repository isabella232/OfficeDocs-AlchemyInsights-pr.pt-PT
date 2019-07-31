---
title: Problemas de início de sessão em aplicações do Office
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
ms.openlocfilehash: 3622a3408b25b43090e9414ae5ffcfc2760264ee
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938302"
---
# <a name="issues-signing-in-to-office-apps"></a>Problemas de início de sessão em aplicações do Office

Para corrigir problemas de início de sessão com aplicações do Office, tente o seguinte:

- Remova todas as contas de trabalho, excepto a conta afectada, utilizando as definições do Windows > **trabalho do Access ou na escola**.
- [Office Limpar credenciais](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) utilizando o Gestor de credenciais do Windows.<br/>
    **Nota:** Os caminhos de registo para o Office 2016 foram alterados para 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Abra uma aplicação do Office, seleccione o **ficheiro** > **conta** > **Terminar sessão**. Em seguida, inicie sessão utilizando uma conta de utilizador com uma licença válida. Para obter informações detalhadas, consulte [contas no Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Para Mac, consulte a ' [não é possível iniciar sessão num 2016 do Office para Mac Apl](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).
- Se ocorrer erros ao estabelecer a ligação utilizando o Office 2013 do Office 365, Active a autenticação moderna de cliente do Office.

Para obter mais informações, consulte:
- [É possível iniciar sessão Office 365, Azure ou Intune](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [Problemas de ligação no início de sessão-in após a actualização do Office de 2016 compilação 16.0.7967 no Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- ["Pedido de desculpa, outra conta da sua organização é ainda tiver sessão iniciada neste computador" no Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [Resolução de problemas de início de sessão com autenticação moderna do Office quando utiliza o ADFS](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)