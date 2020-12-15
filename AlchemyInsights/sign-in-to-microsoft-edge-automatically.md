---
title: Iniciar sôms automaticamente no Microsoft Edge
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
ms.openlocfilehash: 68a1119abd0a3f687b6448bb6e58c6485c239c0f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678812"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Iniciar sôms automaticamente no Microsoft Edge

O Microsoft Edge utiliza a conta predefinida do SISTEMA para assinar automaticamente num utilizador de acordo com a configuração do dispositivo do utilizador. 

Os cenários de cada tipo de configuração do dispositivo e do seu processo de inscrição do utilizador dependente são descritos abaixo:

1. **O dispositivo é híbrido/AAD-J:** Esta opção está disponível no Windows 10, windows de nível inferior e versões de servidor correspondentes. Os utilizadores são automaticamente inscritos nas suas contas Azure Ative Directory (AD)."
2. **O dispositivo está ligado ao domínio**: Esta opção está disponível no Windows 10, no Windows de nível inferior e nas versões correspondentes do servidor. Por padrão, os utilizadores com contas de domínio não são assinados automaticamente; para permitir o seu registo automático, utilize a política **ConfigureOnPremisesAccountAutoSignIn.** Para permitir o registo automático dos utilizadores com contas AD Azure, considere a junção híbrida dos seus dispositivos.
3. **A conta padrão do SISTEMA é uma conta Microsoft**: Esta opção está disponível no Windows 10 RS3 (versão 1709, construa 10.0.16299) e versões posteriores. É pouco provável que o cenário ocorra em dispositivos empresariais. No entanto, se a conta padrão do SISTEMA for uma conta Microsoft, então o Microsoft Edge assinará automaticamente no utilizador com a conta microsoft.
 
 
