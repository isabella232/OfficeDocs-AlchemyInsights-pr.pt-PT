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
- "2559"
ms.openlocfilehash: 57a4df23dc66eaf4c283dde741be6f415939633d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695190"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Correção das aplicações Microsoft 365 "O módulo plataforma fidedigno do computador não está a funcionar corretamente"

Para corrigir este erro, experimente o seguinte:

- Instale as atualizações mais recentes para [windows](https://support.microsoft.com/help/4027667/windows-10-update) e [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Credenciais de Escritório Claro](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) usando Gestor credencial do Windows.<br/>
    **Nota:** Os percursos de registo do Office 2016 mudaram para 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identidade\)
- Experimente o [processo de recuperação](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) do utilizador para corrigir falhas no Módulo de Plataforma Fidedigna (TPM).
- Desa estavido o EnableADAL = 0 utilizando os seguintes passos:  
    1. Clique com o botão Iniciar o Windows, escolha **Executar,** escreva **regedit**e, em seguida, escolha **OK**.
    2. Selecione **Sim** para permitir que o Editor de Registo escora alterações no seu dispositivo.
    3. No Editor de Registos, adicione um valor DWORD de **EnableADAL** com uma definição de **0** em HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identidade.

Para obter mais informações, consulte [os problemas de ligação no sôm-in após a atualização do Office 2016 construir 16.0.7967 no Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).