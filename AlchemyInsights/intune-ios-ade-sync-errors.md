---
title: Erros de sincronização de inscrição automática de dispositivos da Apple
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: d7a9398046a1073e30fdbe2950f750bb55d4fa2f
ms.sourcegitcommit: 87c8d0a1e6668211b9dd5427f98984ccdcadb02d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/17/2020
ms.locfileid: "49714979"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Erros de sincronização de inscrição automática de dispositivos da Apple

"Detetámos que tem uma ou mais fichas ADE/DEP que estão num estado de erro. Até que o estado de erro seja resolvido para cada token afetado, a funcionalidade ADE não funcionará para o mesmo".

Este erro pode manifestar-se de várias formas, incluindo:

1. Os dispositivos não podem sincronizar de ABM/ASM para Intune
2. As atribuições de perfis de inscrição podem estar a falhar
3. Os dispositivos podem não concluir a inscrição do ADE com sucesso

Verifique o erro de sincronização relatado na consola Intune nos **Dispositivos > inscrever dispositivos > fichas do programa de inscrição > da Apple** e rever a seguinte documentação para ver qualquer possível remediação:

[Erros de sincronização ABM/ASM para tokens de inscrição de dispositivos automatizados iOS/iPadOS e macOS](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
