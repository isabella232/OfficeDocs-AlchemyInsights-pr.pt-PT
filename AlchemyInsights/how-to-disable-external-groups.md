---
title: Como desativar grupos externos
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 2159feb4aa3999072de57d76790a2959c7355976
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720779"
---
# <a name="how-to-disable-external-groups"></a>Como desativar grupos externos

As mensagens externas yammer aplicam regras de transporte de câmbio (ETRs), um conjunto de controlos proactivos para impedir que as informações da empresa sejam partilhadas. Para restringir os utilizadores à criação de grupos externos, é necessário configurar uma regra de transporte de intercâmbio (ETR) e, em seguida, configurar a Yammer para usar a regra de Transporte de Intercâmbio para bloquear mensagens externas.
  
Depois de ter criado uma regra no centro de administração Exchange Online, siga estes passos para definir o ETR para aplicar em Yammer:
  
- Inicie sessão na Yammer como administrador verificado, e no centro de **administração yammer,** aceda às Definições de **Segurança de Conteúdo C e Segurança. \> **

- Sob **mensagens externas,** selecione Faça cumprir as suas Regras de Transporte de **Intercâmbio Online (ETRs) em Yammer.**

- Selecione **Guardar**.

Para mais informações, consulte [Desativar mensagens externas numa rede Yammer](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).
  