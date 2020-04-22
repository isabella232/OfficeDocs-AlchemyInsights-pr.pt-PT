---
title: 2491 Mensagens de e-mail de alerta da política 'Phish Delivered devido a inquilino ou utilizador override'
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 2e4efd504304da757687e697ff23374aeea31851
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758940"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Alerte as mensagens de correio eletrónico da política 'Phish Delivered devido a inquilino ou utilizador'

Uma política de alerta padrão chamada "Phish Delivered devido a substituição de inquilino ou utilizador" foi lançada aos inquilinos com licenças ATP P1 e P2 do Office 365 ATP. Se recebeu este alerta, aqui estão os passos para investigar:

1. A partir da mensagem de alerta, clique em **Ver Alerta** para ir à página **alertas** no Centro de Segurança & Compliance.

2. Selecione o alerta para ver a opção de ver a lista de **mensagens** ou **ver mensagens no Explorer**. Ambas as opções levam-no aos detalhes da mensagem, que inclui o ID da Mensagem. Note que a ligação Do Explorador de Ameaças filtrará automaticamente as mensagens que correspondem aos critérios de alerta. Pode ser necessário ajustar o filtro de data no Threat Explorer.

A mensagem de phishing foi entregue devido a uma sobreposição manualmente configurada:

- Um remetente ou domínio permitido definido pelo utilizador.

- Um remetente ou domínio permitido definido pelo administrador numa política anti-correio publicitário não solicitado.

- Um endereço IP permitido numa política de filtro de ligação.

- Uma regra de fluxo de correio (também conhecida como regra de transporte) que é configurada para permitir a entrada de mensagens.

Se acreditar que a mensagem foi incorretamente marcada como phish, utilize o [add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) outlook report Message para enviar amostras de mensagens à Microsoft.
