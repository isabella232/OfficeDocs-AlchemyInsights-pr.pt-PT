---
title: Inscreva-se para Microsoft Edge automaticamente
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
- "8333"
- "9004625"
ms.openlocfilehash: 4e069a1c75caabf3bef7387140edd5650cf966856b888b5c6b5618a603986d6d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050705"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Inscreva-se para Microsoft Edge automaticamente

Microsoft Edge utiliza a conta predefinida do SO para entrar automaticamente num utilizador de acordo com a configuração do dispositivo do utilizador. 

Os cenários de cada tipo de configuração de dispositivos e o res suas processos dependentes de lote de utilizador são descritos abaixo:

- **O dispositivo é híbrido/AAD-J:** esta opção está disponível em Windows 10, versões de servidor Windows de nível inferior e de servidor correspondentes. Os utilizadores têm automaticamente a sua conta Azure Active Directory (AD).
- **O dispositivo está associado ao domínio:** esta opção está disponível em Windows 10, versões de servidor Windows de nível inferior e de servidor correspondentes. Por predefinição, os utilizadores com contas de domínio não têm a sua assinatura automática; para ativar o acesso automático, utilize a política **ConfigureOnPremisesAccountAutoSignIn.** Para ativar o acesso automático a utilizadores com contas Azure AD, considere a associação híbrida dos respetivos dispositivos.
- A conta predefinida do SO é uma conta **Microsoft:** esta opção está disponível no Windows 10 RS3 (versão 1709, comeração 10.0.16299) e versões posteriores. É pouco provável que o cenário ocorra em dispositivos empresariais. No entanto, se a conta predefinida do SO for uma conta Microsoft, Microsoft Edge a sua conta irá entrar automaticamente no utilizador com a conta Microsoft.
 
 
