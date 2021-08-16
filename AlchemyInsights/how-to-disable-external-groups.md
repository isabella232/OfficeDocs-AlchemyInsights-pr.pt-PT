---
title: Como desativar Grupos Externos
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 9c513da49dc953b4ae76bb06854e33232ec40e11151f11ade33c3080092aa598
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54015631"
---
# <a name="how-to-disable-external-groups"></a>Como desativar Grupos Externos

Yammer mensagens externas aplicam-se Exchange de Transporte (ETR), um conjunto de controlos proativos para impedir a partilha de informações da empresa. Para impedir que os utilizadores criem grupos externos, tem de configurar uma regra de transporte do Exchange (ETR) e, em seguida, configurar o Yammer para utilizar a regra de Transporte do Exchange para bloquear mensagens externas.
  
Assim que tiver criado uma regra no Exchange Online de administração, siga estes passos para definir o ETR para ser aplicado no Yammer:
  
- Indique sessão no Yammer como um administrador verificado e, no centro de administração do **Yammer,** aceda a Conteúdo C e Segurança **\> Definições.**

- Em **Mensagens Externas, selecione** Impor as Exchange Online Exchange de Transporte **(ETRs) no Yammer.**

- Selecione **Guardar**.

Para obter mais informações, [consulte Desativar mensagens externas numa Yammer Rede](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).
  