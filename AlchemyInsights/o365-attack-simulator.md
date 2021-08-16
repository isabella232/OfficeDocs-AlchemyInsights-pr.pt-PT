---
title: Simulador de Ataque 2681 no Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: b173c6eb3bbbd1beba3b59878ae12bbe7684d0447a16fef746e5b97b82349e53
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54065295"
---
# <a name="attack-simulator-in-microsoft-365"></a>Simulador de Ataque no Microsoft 365

- Não tem o Simulador de Ataque? O Simulador de **Ataque necessita do Microsoft Defender Office 365 Plano 2** ou Office 365 Enterprise **E5.** O Simulador de **Ataque não** está incluído no Microsoft Defender para Office 365 Plano 1, Office 365 Enterprise E3 ou Microsoft 365 Apps para Pequenas e Médias Empresas subscrições.

- A conta que utiliza para iniciar ataques simulados requer permissões de administrador global ou administrador de segurança e a autenticação multifator (MFA). Para obter mais informações sobre os requisitos do Simulador de Ataque, [consulte este tópico.](/microsoft-365/security/office-365-security/attack-simulator)

- As coisas importantes a saber sobre **simulações de ataque de Forçar Palavra-passe Brute:**

  - Se a conta de destino tiver a autenticação mfa ativada e a palavra-passe tiver sido corretamente adivinhar, a conta não será mostrada como comprometida (o segundo fator de autenticação estará incompleto).

  - O ficheiro de palavra-passe não pode ter mais de 10 MB. Utilize uma palavra-passe por linha e inclua uma linha em branco (sinal de retorno) após a última palavra-passe na lista.

- Informações importantes sobre as **simulações de anexação de Phishing spear:**

  - Por predeleção, não pode fornecer um valor personalizado para o URL do servidor de início de sessão de **Phishing.**

  - Se um destinatário [](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) utilizar o adicionar Ativar a Mensagem do Relatório para denunciar a mensagem como phishing, poderá não receber alertas da mensagem (porque se trata de um ataque simulado).

- Relatórios: quando o ataque simulado estiver concluído, pode clicar em Detalhes **do Ataque** para ver o relatório.

- Para obter instruções detalhadas e novas funcionalidades no Simulador de Ataque, consulte [Simulador](/microsoft-365/security/office-365-security/attack-simulator)de Ataque Microsoft 365 .
