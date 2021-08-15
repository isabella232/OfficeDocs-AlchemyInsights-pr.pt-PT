---
title: Erros de sincronização da Inscrição Automática de Dispositivos da Apple
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
ms.openlocfilehash: 1664a26b313c4a38c9c6d78cdb89997749ba175fd3dd72f278e99bbd50b0ee84
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013759"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Erros de sincronização da Inscrição Automática de Dispositivos da Apple

"Detetamos que tem um ou mais Tokens ADE/DEP que estão num estado de erro. Até que o estado de erro seja resolvido para cada token afetado, a funcionalidade ADE não irá funcionar como esperado.".

Este erro pode manifestar-se de várias formas, incluindo:

1. Os dispositivos podem não ser sincronizados a partir da ABM/ASM para o Intune
2. As atribuições de perfis de inscrição podem estar a falhar
3. Os dispositivos podem não concluir a inscrição ADE com êxito

Verifique se o erro de sincronização foi comunicado na consola do Intune em Dispositivos > Inscrever Dispositivos > inscrever-se na **Apple > tokens** do programa de inscrição .

Uma das causas mais comuns do erro de sincronização é a expiração do token atual. Em muitos casos, a renovação do token afetado irá resolver o problema.

Se um ou mais dos seus tokens expirou, consulte a seguinte documentação para ajudá-lo a renová-los conforme adequado:

[Renovar um token de Inscrição de Dispositivos Automatizados](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

Além disso, pode ver a seguinte documentação para ver possíveis remediações de outros erros que causam falhas na sincronização de tokens:

[Erros de Sincronização ABM/ASM para iOS/iPadOS e Tokens de Inscrição de Dispositivos Automatizados no macOS](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[Erros de Sincronização ABM/ASM para iOS/iPadOS e Tokens de Inscrição de Dispositivos Automatizados no macOS](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
