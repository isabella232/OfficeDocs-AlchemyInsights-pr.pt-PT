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
- "2559"
ms.openlocfilehash: 5f500ecf1f779fb1be4d257fd050a3ad054087dc
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938304"
---
# <a name="fixing-the-office-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Corrigir a mensagem de "módulo de plataforma fidedigna do computador não está a funcionar correctamente" de aplicações do Office

Para corrigir este erro, tente o seguinte:

- Instale as actualizações mais recentes para o [Windows](https://support.microsoft.com/help/4027667/windows-10-update) e [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Office Limpar credenciais](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) utilizando o Gestor de credenciais do Windows.<br/>
    **Nota:** Os caminhos de registo para o Office 2016 foram alterados para 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Tente o [processo de recuperação de utilizador](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) para corrigir falhas de Trusted Platform Module (TPM).
- Definir o EnableADAL = 0, utilizando os seguintes passos:  
    1. Botão direito do rato no botão Iniciar do Windows, seleccione **Executar**, escreva **regedit**e, em seguida, escolha **' OK '**.
    2. Seleccione **Sim** para permitir que o Editor de registo para efectuar alterações ao dispositivo.
    3. No Editor de registo, adicione um valor DWORD de **EnableADAL** com uma definição de **0** em HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Para mais informações, consulte [problemas de ligação no início de sessão-in após a actualização do Office de 2016 compilação 16.0.7967 10 do Windows](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).