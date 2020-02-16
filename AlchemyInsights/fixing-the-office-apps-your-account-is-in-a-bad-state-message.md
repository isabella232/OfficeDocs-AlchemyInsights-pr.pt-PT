---
title: Fixação das Aplicações do Office A sua conta está numa mensagem de mau estado
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: e591c56dd207a5bcb3979be3f66052121100b162
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/27/2019
ms.locfileid: "41969693"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a>Corrigir as aplicações do Office "A sua conta está em mau estado" erro

Para corrigir este erro, tente as seguintes opções no computador afetado:

- Abra uma aplicação do Office, selecione **File** > **Account** > Sign out de todas as**contas**. Volte a fazer o sessão utilizando uma conta de utilizador com uma licença válida. Para obter informações [detalhadas,](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9)consulte contas no Office .
- [Credenciais de escritório claro](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) usando O Gestor Credencial do Windows.<br>
  **Nota:** As vias de registo do Office 2016 mudaram para 16,0. Por exemplo, \Software\Microsoft\Office\16.0\Common\Identity\
- No computador afetado, coloque o EnableADAL = 0 utilizando os seguintes passos:  
     1. Clique no botão Windows e selecione **Executar**. Na caixa **Aberta,** escreva **regedite,** e, em seguida, selecione **OK**.
     2. Selecione **Sim** quando solicitado para permitir que o Editor de Registo faça alterações no seu dispositivo.
    3. No Editor de Registo, adicione um valor DWORD de EnableADAL com uma definição de 0 em HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.
- Se o erro ocorrer durante a ligação ao Office 365 utilizando o Office 2013, ative a [autenticação moderna](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) para o cliente do Office.

Para mais informações, consulte [Como resolver aplicações não-navegadoras que não podem iniciar sessão no Office 365, Azure ou Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).

