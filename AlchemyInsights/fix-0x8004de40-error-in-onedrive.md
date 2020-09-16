---
title: Corrigir erro 0x8004de40 no OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: b9bd6dff48f78063e3d47f5fe2f834f59eb9868a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745141"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Corrigir erro 0x8004de40 no OneDrive

Se receber um erro de 0x8004de40 com o OneDrive:

- Reinicie o computador afetado enquanto estiver ligado ao seu domínio acitve Directory.
- Se um reboot não corrigir o problema, un un unin e rejoine o seu dispositivo a partir de Azure AD. 

**Nota:** Deve estar na sua rede corporativa durante a realização destes passos. Não execute estes passos quando não é capaz de se conectar à sua infraestrutura corporativa (por exemplo, durante a viagem). 

- Abra um pedido de comando elevado. 
- Para abrir um pedido de comando elevado, clique em - **Iniciar**, clique com o botão direito **Command Prompt**e, em seguida, clique em Executar **como administrador**.
- Tipo *dsregcmd /leave* and press **Enter**.
- Quando estiver concluído, *escreva /junte-se* e prima **Enter**.
- Quando estiver completo, feche o aviso de comando.
- Reinicie o computador e inicie sessão no OneDrive.