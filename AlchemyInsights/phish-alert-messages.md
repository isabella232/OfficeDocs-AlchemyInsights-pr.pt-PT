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
ms.openlocfilehash: 2b373423cf3e63b76a62465dd62076c023580e94
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544589"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Alertar mensagens de e-mail da política "Phish Entregue devido a um inquilino ou a uma override de utilizador"

Uma política de alerta predefinida denominada "Phish Entregue devido a um inquilino ou a uma override de utilizador" foi lançada para os inquilinos com o Microsoft Defender para Office 365 licenças do Office 365 P1 e P2. Se recebeu este alerta, eis os passos para investigar:

1. A partir da mensagem de alerta, clique **em Ver** Alerta para ir para a **página Alertas** no Centro de conformidade & Segurança.

2. Selecione o alerta para ver a opção ver **a lista de mensagens** ou Ver mensagens no **Explorador.** Ambas as opções levam-no aos detalhes da mensagem, que inclui o ID da Mensagem. Tenha em atenção que a ligação Explorador de Ameaças irá filtrar automaticamente as mensagens que correspondem aos critérios de alerta. Poderá ter de ajustar o filtro de datas no Explorador de Ameaças.

A mensagem de phishing foi entregue devido a uma override configurada manualmente:

- Um remetente ou domínio permitido definido pelo utilizador.

- Um remetente ou domínio permitido definido pelo administrador numa política antisspam.

- Um endereço IP permitido numa política de filtro de ligação.

- Uma regra de fluxo de correio (também conhecida como regra de transporte) que está configurada para permitir mensagens.

Se acredita que a mensagem foi marcada incorretamente como phish, utilize o [Outlook-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) Report Message (Mensagem de Relatório) para submeter exemplos de mensagens à Microsoft.
