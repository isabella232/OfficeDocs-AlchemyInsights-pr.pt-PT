---
title: Como desactivar grupos externo
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
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/04/2019
ms.locfileid: "36739504"
---
# <a name="how-to-disable-external-groups"></a>Como desactivar grupos externo

Do Yammer mensagens externas aplicam regras de transporte de troca (ETRs), um conjunto de controlos proactivas para impedir que as informações da empresa a ser partilhado. Para impedir que os utilizadores a criação de grupos externos, tem de configurar uma regra de transporte do Exchange (ETR) e, em seguida, do Yammer para utilizar a regra de transporte do Exchange para bloquear mensagens externas.
  
Depois de criar uma regra no Centro de administração Exchange Online, siga estes passos para definir ETR para aplicar no Yammer:
  
- Iniciar sessão no Yammer como um administrador verificado e, **do Yammer Centro de administração**, vá para C **conteúdo e de segurança \> as definições de segurança.**

- Em **Processamento de mensagens externo**, seleccione **impor as regras de transporte do Exchange por Exchange Online (ETRs) no Yammer.**

- Selecione **Guardar**.

Para mais informações, consulte [Desactivar externos de mensagens numa rede do Yammer](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).
  