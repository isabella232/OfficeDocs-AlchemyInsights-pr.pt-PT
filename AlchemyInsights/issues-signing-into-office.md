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
- "2574"
ms.openlocfilehash: f8f2824cc4a575ab7d7c9adec5b75e5955ec9fb5
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744657"
---
# <a name="issues-signing-into-microsoft-365-apps"></a>Problemas ao entrar no Microsoft 365 Apps

Nota: se estiver a utilizar uma versão mais antiga do Windows (por exemplo, Windows 7 SP1, Windows Server [](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) 2008 R2), utilize a correção fácil para ativar o TLS 1.2 como predefinição. Para obter mais informações, consulte Update [to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).

Para corrigir problemas de início de sessão no Microsoft 365 Apps, experimente as seguintes opções no computador afetado:  

- Para Windows, consulte [Recomendações a resolução de problemas comuns de lote de lote](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues)
- Para Mac, consulte [Não é possível entrar numa aplicação Office 2016 para Mac Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)

**Sugestão** Em computadores Windows, podemos diagnosticar e corrigir automaticamente vários problemas comuns de início de sessão do Office. Transfira e execute o **[Assistente de Recuperação e Suporte da Microsoft](https://aka.ms/SaRA-OfficeSignInScenario)** para utilizar a nossa ferramenta automatizada.

**Nota:** Não é recomendado desativar a Autenticação Moderna (ADAL) ou a Gestão de Conta Web (WAM) para corrigir problemas de arranque ou de **ativação.** Se os erros ocorrerem ao ligar ao Microsoft 365 utilizando o Office 2013, certifique-se de que ativa a autenticação moderna Office cliente. [](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)

Para ações de remoção de problemas específicas, consulte:

[Problemas de conexão no início de sessão após atualização para o Office 2016 compilação 16.0.7967 no Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)  

[Não pode inscrever-se na sua conta organizacional, como o Office 365, o Azure ou o Intune](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)

[Como refletir problemas com aplicações que não são do browser que não conseguem entrar no Office 365, no Azure ou no Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1?ui=en-US&rs=en-US&ad=US)

[Pedido repetidamente para as credenciais no Office](https://docs.microsoft.com/office365/troubleshoot/authentication/access-denied-when-connect-to-office-365)