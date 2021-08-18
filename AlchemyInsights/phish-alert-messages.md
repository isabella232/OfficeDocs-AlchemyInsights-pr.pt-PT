---
title: 2491 Alertar mensagens de e-mail da política "Phish Entregue devido a inquilino ou utilizador de override"
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
ms.openlocfilehash: 90b078147bbb1e60cba0a2de6e49a862469f93aa
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316369"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Alertar mensagens de e-mail da política "Phish Entregue devido a um inquilino ou a uma override de utilizador"

Está disponível uma política de alerta predefinida denominada **Phish Entregue** devido a uma sobresserção de utilizador ou inquilino em organizações com o Microsoft Defender para Office 365 licenças P1 e P2. Se recebeu este alerta, eis os passos para investigar:

1. A partir da mensagem de alerta, **clique em** Ver Alerta para ir para a **página Alertas** no portal Microsoft 365 Defender alertas.

2. Selecione o alerta para ver a opção ver **a lista de mensagens** ou Ver mensagens no **Explorador.** Ambas as opções levam-no aos detalhes da mensagem, que inclui o ID da Mensagem. Tenha em atenção que a ligação Explorador de Ameaças irá filtrar automaticamente as mensagens que correspondem aos critérios de alerta. Poderá ter de ajustar o filtro de datas no Explorador de Ameaças.

A mensagem de phishing foi entregue devido a uma override configurada manualmente:

- Um remetente ou domínio permitido definido pelo utilizador.
- Um remetente ou domínio permitido definido pelo administrador numa política antisspam.
- Um endereço IP permitido numa política de filtro de ligação.
- Uma regra de fluxo de correio (também conhecida como regra de transporte) que está configurada para permitir mensagens.

Se acredita que a mensagem foi marcada incorretamente como phishing, utilize [a submissão](https://docs.microsoft.com/microsoft-365/security/office-365-security/admin-submission) administrador para comunicar a mensagem à Microsoft.

Os utilizadores podem utilizar [o add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) Mensagem de Relatório ou o Outlook report phishing para submeter exemplos de mensagens à Microsoft.
