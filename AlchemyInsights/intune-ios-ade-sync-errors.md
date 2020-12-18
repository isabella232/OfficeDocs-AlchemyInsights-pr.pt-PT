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
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="c7119-102">Erros de sincronização de inscrição automática de dispositivos da Apple</span><span class="sxs-lookup"><span data-stu-id="c7119-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="c7119-103">"Detetámos que tem uma ou mais fichas ADE/DEP que estão num estado de erro.</span><span class="sxs-lookup"><span data-stu-id="c7119-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="c7119-104">Até que o estado de erro seja resolvido para cada token afetado, a funcionalidade ADE não funcionará para o mesmo".</span><span class="sxs-lookup"><span data-stu-id="c7119-104">Until the error state is resolved for each affected token, the ADE functionality will not work for the same”.</span></span>

<span data-ttu-id="c7119-105">Este erro pode manifestar-se de várias formas, incluindo:</span><span class="sxs-lookup"><span data-stu-id="c7119-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="c7119-106">Os dispositivos não podem sincronizar de ABM/ASM para Intune</span><span class="sxs-lookup"><span data-stu-id="c7119-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="c7119-107">As atribuições de perfis de inscrição podem estar a falhar</span><span class="sxs-lookup"><span data-stu-id="c7119-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="c7119-108">Os dispositivos podem não concluir a inscrição do ADE com sucesso</span><span class="sxs-lookup"><span data-stu-id="c7119-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="c7119-109">Verifique o erro de sincronização relatado na consola Intune nos **Dispositivos > inscrever dispositivos > fichas do programa de inscrição > da Apple** e rever a seguinte documentação para ver qualquer possível remediação:</span><span class="sxs-lookup"><span data-stu-id="c7119-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens** and review the following documentation to see any potential remediation:</span></span>

[<span data-ttu-id="c7119-110">Erros de sincronização ABM/ASM para tokens de inscrição de dispositivos automatizados iOS/iPadOS e macOS</span><span class="sxs-lookup"><span data-stu-id="c7119-110">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
