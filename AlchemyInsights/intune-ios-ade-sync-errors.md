---
title: Erros de sincronização de inscrição automática de dispositivos da Apple
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: 912c9e56b4c468fb333769f15bd7c212594dc11a
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448933"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Erros de sincronização de inscrição automática de dispositivos da Apple

"Detetámos que tem uma ou mais fichas ADE/DEP que estão num estado de erro. Até que o estado de erro seja resolvido para cada token afetado, a funcionalidade ADE não funcionará como esperado."

Este erro pode manifestar-se de várias formas, incluindo:

1. Os dispositivos não podem sincronizar de ABM/ASM para Intune
2. As atribuições de perfis de inscrição podem estar a falhar
3. Os dispositivos podem não concluir a inscrição do ADE com sucesso

Verifique o erro de sincronização relatado na consola Intune nos **Dispositivos > inscrever dispositivos > fichas do programa de inscrição > da Apple**.

Uma das causas mais comuns de erro de sincronização é a expiração do token atual. Em muitos casos, a renovação do símbolo afetado resolverá a questão.

Se uma ou mais das suas fichas tiver expirado, consulte a seguinte documentação para ajudá-lo a renová-las conforme apropriado:

[Renovar um token de inscrição de dispositivo automatizado](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

Além disso, pode ver a seguinte documentação para ver possíveis reparações para outros erros que causam falhas de sincronização de fichas:

[Erros de sincronização ABM/ASM para tokens de inscrição de dispositivos automatizados iOS/iPadOS e macOS](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[Erros de sincronização ABM/ASM para tokens de inscrição de dispositivos automatizados iOS/iPadOS e macOS](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
