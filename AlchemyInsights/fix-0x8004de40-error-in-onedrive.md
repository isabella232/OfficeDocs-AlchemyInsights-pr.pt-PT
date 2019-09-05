---
title: Corrigir o erro de 0x8004de40 em OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: aa0e0a63ac1e365a7cdce018626740446040a664
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/04/2019
ms.locfileid: "36755859"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Corrigir o erro de 0x8004de40 em OneDrive

Se receber um erro de 0x8004de40 com OneDrive:

- Reinicie o computador afectado enquanto estiver ligado ao domínio do directório Acitve.
- Se reiniciar o computador não corrigir o problema, desligar e voltar a aderir o dispositivo do Azure AD. 

**Nota**: deve estar na rede da empresa ao efectuar estes passos. Não efectue estes passos quando não conseguir estabelecer ligação com a infra-estrutura da empresa (por exemplo, quando estou em viagem). 

- Abra uma linha de comandos elevada. 
- Para abrir uma linha de comandos elevada, clique - **Iniciar**, clique em **linha de comandos**e, em seguida, clique em **Executar como administrador**.
- Escreva *dsregcmd /leave* e prima **Enter**.
- Quando tiver terminado, escreva *dsregcmd /join* e prima **Enter**.
- Quando tiver terminado, feche a linha de comandos.
- Reinicie o computador e inicie sessão em OneDrive.