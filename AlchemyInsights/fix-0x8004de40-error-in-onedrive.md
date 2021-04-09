---
title: Corrigir erro de 0x8004de40 no OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649759"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Corrigir erro de 0x8004de40 no OneDrive

Se estiver a executar o Windows 7 e receber este erro, [atualize para ativar o TLS 1.1 e o TLS 1.2 como protocolos seguros predefinidos no WinHTTP no Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).

Se estiver a executar o Windows 10 e receber um erro 0x8004de40 com o OneDrive:

- Reinicie o computador afetado enquanto estiver ligado ao seu domínio acitve Directory.
- Se um reboot não corrigir o problema, un un unin e rejoine o seu dispositivo a partir de Azure AD. 

**Nota:** Deve estar na sua rede corporativa durante a realização destes passos. Não execute estes passos quando não estiver ligado à sua infraestrutura corporativa (por exemplo, durante a viagem). 

1. Abra uma solicitação de comando elevada selecionando **Iniciar**, clique com o botão direito **Command Prompt** e, em seguida, selecione Executar **como administrador**.

1. Tipo *dsregcmd /leave* and press **Enter**.

1. Quando estiver concluído, *escreva /junte-se* e prima **Enter**.

1. Quando estiver completo, feche o aviso de comando.

1. Reinicie o computador e inicie sessão no OneDrive.