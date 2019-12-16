---
title: Corrigir erro 0x8004de40 no OneDrive
ms.author: pebaum
author: pebaum
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 48b29f57763ca22a71a23b2afddcac0e8e8a95db
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052048"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Corrigir erro 0x8004de40 no OneDrive

Se você receber um erro 0x8004de40 com OneDrive:

- Reiniciar o computador afetado enquanto estiver conectado ao seu domínio acitve diretório.
- Se uma reinicialização não corrigir o problema, unjoin e voltar ao seu dispositivo a partir de AD Azure. 

**Nota:** Você deve estar em sua rede corporativa durante a execução dessas etapas. Não execute essas etapas quando você não é capaz de se conectar à sua infraestrutura corporativa (por exemplo, durante a viagem). 

- Abra uma alerta de comando elevado. 
- Para abrir um alerta de comando elevado, clique em - **Comece,** clique à direita **no Comando Prompt**e, em seguida, clique em Correr como **administrador.**
- Tipo *dsregcmd /leave* and press **Enter**.
- Quando completo, tipo *dsregcmd /join* e **pressione Entre.**
- Quando estiver completo, feche o alerta de comando.
- Reiniciar o computador, e entrar em OneDrive.