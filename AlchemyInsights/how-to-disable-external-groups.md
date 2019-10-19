---
title: Como desabilitar grupos externos
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: b2328ea85d3ff6ec722cc56d8a46395d8438f79c
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/18/2019
ms.locfileid: "36739504"
---
# <a name="how-to-disable-external-groups"></a>Como desabilitar grupos externos

O sistema de mensagens externas do Yammer aplica as regras de transporte do Exchange (ETRs), um conjunto de controles pró-ativos para impedir que as informações da empresa sejam compartilhadas. Para restringir os usuários de criar grupos externos, você precisa configurar uma regra de transporte do Exchange (ETR) e, em seguida, configurar o Yammer para usar a regra de transporte do Exchange para bloquear mensagens externas.
  
Depois de criar uma regra no centro de administração do Exchange Online, siga estas etapas para definir ETR para aplicar no Yammer:
  
- Faça logon no Yammer como um administrador verificado e no centro de **Administração do Yammer**, vá para **configurações de segurança de \> conteúdo e segurança** do C.

- Em **mensagens externas**, selecione **impor suas regras de transporte do Exchange Online Exchange (ETRS) no Yammer.**

- Selecione **Guardar**.

Para obter mais informações, consulte [desabilitar mensagens externas em uma rede Yammer](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).
  