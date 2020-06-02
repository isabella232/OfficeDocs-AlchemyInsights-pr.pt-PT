---
title: 2681 Simulador de ataque na Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 3dae4768ca62757ce7f92dfc527078c963d72742
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506749"
---
# <a name="attack-simulator-in-microsoft-365"></a>Simulador de ataque na Microsoft 365

- Estás a perder o Simulador de Ataque? O Simulador de Ataque requer **o Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** ou **o Office 365 Enterprise E5**. O Simulador de Ataque **não** está incluído no Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), no Office 365 Enterprise E3 ou em quaisquer aplicações da Microsoft 365 para subscrições empresariais.

- A conta que utiliza para lançar ataques simulados requer permissões globais de administrador ou administrador de segurança e autenticação de vários fatores (MFA). Para obter mais informações sobre os requisitos do Simulador de Ataque, consulte [este tópico.](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)

- Coisas importantes a saber sobre simulações de ataque de password da **Força Bruta:**

  - Se a conta-alvo tiver MFA ativada e a palavra-passe foi adivinhada corretamente, a conta não será apresentada como comprometida (o segundo fator de autenticação estará incompleto).

  - O ficheiro de senha não pode ser maior que 10 MB. Use uma palavra-passe por linha e inclua uma linha em branco (retorno do transporte) após a última palavra-passe da lista.

- Coisas importantes a saber sobre simulações de **phishing de lança:**

  - Por design, não é possível fornecer um valor personalizado para **o URL do servidor de login do Phishing.**

  - Se um destinatário utilizar [o add-in 'Ativar a mensagem's](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) reporte a mensagem como phishing, poderá não receber alertas para a mensagem (porque se trata de um ataque simulado).

- Relatórios: Após o ataque simulado estar completo, pode clicar em **Detalhes de Ataque** para ver o relatório.

- Para obter instruções detalhadas e novas funcionalidades no Simulador de Ataque, consulte [o Simulador de Ataque na Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
