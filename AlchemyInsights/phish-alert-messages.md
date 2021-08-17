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
ms.openlocfilehash: 2e24f489292f38b5e9cacc8b9bfe5730ebfc71ce5e3004be479134ef6c791a12
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/11/2021
ms.locfileid: "57899343"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Alertar mensagens de e-mail da política "Phish Entregue devido a um inquilino ou a uma override de utilizador"

Está disponível uma política de alerta predefinida denominada Phish Entregue devido a uma **override** de utilizador ou inquilino em organizações com o Microsoft Defender para Office 365 licenças P1 e P2. Se recebeu este alerta, eis os passos para investigar:

1. A partir da mensagem de alerta, **clique em** Ver Alerta para ir para a **página Alertas** no Microsoft 365 Defender portal.

2. Selecione o alerta para ver a opção ver **a lista de mensagens** ou Ver mensagens no **Explorador.** Ambas as opções levam-no aos detalhes da mensagem, que inclui o ID da Mensagem. Tenha em atenção que a ligação Explorador de Ameaças irá filtrar automaticamente as mensagens que correspondem aos critérios de alerta. Poderá ter de ajustar o filtro de datas no Explorador de Ameaças.

A mensagem de phishing foi entregue devido a uma override configurada manualmente:

- Um remetente ou domínio permitido definido pelo utilizador.
- Um remetente ou domínio permitido definido pelo administrador numa política antisspam.
- Um endereço IP permitido numa política de filtro de ligação.
- Uma regra de fluxo de correio (também conhecida como regra de transporte) que está configurada para permitir mensagens.

Se acredita que a mensagem foi marcada incorretamente como phishing, utilize [a submissão](https://docs.microsoft.com/microsoft-365/security/office-365-security/admin-submission) administrador para comunicar a mensagem à Microsoft.

Os utilizadores podem utilizar [o add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) Mensagem de Relatório ou o Outlook report phishing para submeter exemplos de mensagens à Microsoft.
