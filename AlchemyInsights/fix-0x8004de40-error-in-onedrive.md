---
title: Corrigir erro 0x8004de40 no OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 5da4271f242597b195ef61d553fd4a2ffb313025
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716039"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Corrigir erro 0x8004de40 no OneDrive

Se receber um erro 0x8004de40 com o OneDrive:

- Reinicie o computador afetado enquanto está ligado ao seu domínio de Diretório Acitve.
- Se um reboot não resolver o problema, desadere e volte a juntar-se ao seu dispositivo a partir de Azure AD. 

**Nota:** Deve estar na sua rede corporativa enquanto realiza estes passos. Não execute estes passos quando não conseguir ligar-se à sua infraestrutura corporativa (por exemplo, durante a viagem). 

- Abra um pedido de comando elevado. 
- Para abrir um pedido de comando elevado, clique em **- Iniciar**, clique à direita No Pedido de **Comando**, e, em seguida, clique em Executar **como administrador**.
- Digite *dsregcmd /leave* e **pressione Enter**.
- Quando estiver concluído, escreva *dsregcmd /junte* e prima **Enter**.
- Quando estiver concluído, feche o pedido de comando.
- Reinicie o computador e entre no OneDrive.