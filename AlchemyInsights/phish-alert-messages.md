---
title: 2491 Alerte as mensagens de correio da política "Phish Delivered devido à política de inquilina ou substituição de utilizador"
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 5b5faa08542cb5878107f10afb34427f636562ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728622"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Alerte as mensagens de correio da política "Phish Delivered devido à política de inquilina ou substituição de utilizador"

Uma política de alerta padrão denominada "Phish Delivered devido a inquilina ou substituição de utilizador" foi lançada para inquilinos com licenças Do Office 365 ATP P1 e P2. Se recebeu este alerta, aqui estão os passos para investigar:

1. A partir da mensagem de alerta, clique em **Ver Alerta** para ir à página **Alertas** no Centro de Conformidade & de Segurança.

2. Selecione o alerta para ver a opção de visualizar a **lista de mensagens** ou **ver mensagens no Explorer**. Ambas as opções levam-no aos detalhes da mensagem, que inclui o ID da mensagem. Note que a ligação Exploradora de Ameaças filtrará automaticamente as mensagens que correspondem aos critérios de alerta. Pode ser necessário ajustar o filtro de datas no Explorador de Ameaças.

A mensagem de phishing foi entregue devido a uma sobreposição configurada manualmente:

- Um remetente ou domínio permitido definido pelo utilizador.

- Um remetente ou domínio permitido definido pelo administrador numa política anti-correio publicitário não-correio eletrónico.

- Um endereço IP permitido numa política de filtro de ligação.

- Uma regra de fluxo de correio (também conhecida como regra de transporte) que está configurada para permitir a entrada de mensagens.

Se acredita que a mensagem foi incorretamente marcada como phish, utilize o [add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) da Mensagem do Relatório do Outlook para enviar amostras de mensagens à Microsoft.
