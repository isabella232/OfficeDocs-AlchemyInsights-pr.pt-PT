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
- "2559"
ms.openlocfilehash: b0789a54f48b2850c1dad8651a8209449c805784bea96799f05e67c4bc43fdb0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53986902"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Corrigir as aplicações Microsoft 365 mensagem "O módulo de Plataforma Fideder do seu computador não está a funcionar corretamente"

Para corrigir este erro, experimente o seguinte:

- Instale as atualizações mais [recentes Windows](https://support.microsoft.com/help/4027667/windows-10-update) e [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Limpe Office de credenciais utilizando](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) o Windows de Credenciais.<br/>
    **Nota:** Os caminhos de registo Office 2016 mudaram para 16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Experimente o [processo de recuperação de](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) utilizadores para corrigir falhas do Módulo de Plataforma De Confiança (TPM).
- Defina EnableADAL = 0 ao seguir os seguintes passos:  
    1. Clique com o botão direito do rato Windows Iniciar, **selecionar Executar**, escreva **regedit** e, em seguida, selecionar **OK.**
    2. **Selecione** Sim para permitir que o Editor de Registo faça alterações ao seu dispositivo.
    3. No Editor de Registo, adicione um valor DWORD de **EnableADAL** com uma definição **de 0** em HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Para obter mais informações, consulte Problemas de ligação ao inscrever-se após a atualização para [a comarca 16.0.7967](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)do Office Windows 10 .