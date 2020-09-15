---
title: Como desativar grupos externos
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
ms.openlocfilehash: f7a1bbda3a54d2662bdfe21cda961c32456edb82
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704139"
---
# <a name="how-to-disable-external-groups"></a>Como desativar grupos externos

A mensagem externa da Yammer aplica regras de transporte de câmbio (ETRs), um conjunto de controlos pró-ativos para impedir que a informação da empresa seja partilhada. Para restringir os utilizadores à criação de grupos externos, é necessário configurar uma regra de transporte de intercâmbio (ETR) e, em seguida, configurar a Yammer para usar a regra do Transporte de Intercâmbio para bloquear mensagens externas.
  
Uma vez criada uma regra no Centro de Administração Exchange Online, siga estes passos para definir ETR para aplicar em Yammer:
  
- Inicie sessão no Yammer como administrador verificado, e no **centro de administração Yammer,** vá para C **Conteúdo e \> Definições de Segurança.**

- Em **Mensagens Externas,** **selecione Impor as suas Regras de Transporte de Intercâmbio Online (ETRs) em Yammer.**

- Selecione **Guardar**.

Para obter mais informações, consulte [Mensagens externas desativada numa rede Yammer](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).
  