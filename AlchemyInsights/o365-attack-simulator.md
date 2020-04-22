---
title: Simulador de ataque 2681 na Microsoft 365
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
ms.openlocfilehash: 74bd2dd62b24aaf6c9d7b387ab1d97ddab31e902
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713477"
---
# <a name="attack-simulator-in-microsoft-365"></a>Simulador de ataque na Microsoft 365

- Estás a perder o Simulador de Ataque? O Simulador de Ataque requer o **Office 365 Advanced Threat Protection Plan 2 (PLANO ATP 2)** ou **o Office 365 Enterprise E5**. O Attack Simulator **não** está incluído no Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3 ou em quaisquer Aplicações Microsoft 365 para subscrições de negócios.

- A conta que utiliza para lançar ataques simulados requer permissões de administrador global ou administrador de segurança e autenticação de vários fatores (MFA). Para mais informações sobre os requisitos do Simulador de Ataque, consulte [este tópico](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).

- Coisas importantes a saber sobre simulações de ataque de **palavra-passe** da Força Bruta:

  - Se a conta-alvo tiver MFA ativada e a palavra-passe tiver sido adivinho corretamente, a conta não aparecerá como comprometida (o segundo fator de autenticação estará incompleto).

  - O ficheiro de senha não pode ser maior que 10 MB. Utilize uma palavra-passe por linha e inclua uma linha em branco (retorno do transporte) após a última palavra-passe da lista.

- Coisas importantes a saber sobre **spear phishing** anexam simulações:

  - Por design, não é possível fornecer um valor personalizado para o URL do servidor de **login**de phishing .

  - Se um destinatário utilizar o [add-in Enable the Report Message](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) para relatar a mensagem como phishing, poderá não receber alertas para a mensagem (porque se trata de um ataque simulado).

- Relatórios: Após o ataque simulado estar completo, pode clicar em Detalhes de **Ataque** para ver o relatório.

- Para obter instruções detalhadas e novas funcionalidades no Simulador de Ataque, consulte [o Simulador de Ataque na Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
