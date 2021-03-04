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
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="784ae-102">Erros de sincronização de inscrição automática de dispositivos da Apple</span><span class="sxs-lookup"><span data-stu-id="784ae-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="784ae-103">"Detetámos que tem uma ou mais fichas ADE/DEP que estão num estado de erro.</span><span class="sxs-lookup"><span data-stu-id="784ae-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="784ae-104">Até que o estado de erro seja resolvido para cada token afetado, a funcionalidade ADE não funcionará como esperado."</span><span class="sxs-lookup"><span data-stu-id="784ae-104">Until the error state is resolved for each affected token, the ADE functionality will not work as expected.”.</span></span>

<span data-ttu-id="784ae-105">Este erro pode manifestar-se de várias formas, incluindo:</span><span class="sxs-lookup"><span data-stu-id="784ae-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="784ae-106">Os dispositivos não podem sincronizar de ABM/ASM para Intune</span><span class="sxs-lookup"><span data-stu-id="784ae-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="784ae-107">As atribuições de perfis de inscrição podem estar a falhar</span><span class="sxs-lookup"><span data-stu-id="784ae-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="784ae-108">Os dispositivos podem não concluir a inscrição do ADE com sucesso</span><span class="sxs-lookup"><span data-stu-id="784ae-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="784ae-109">Verifique o erro de sincronização relatado na consola Intune nos **Dispositivos > inscrever dispositivos > fichas do programa de inscrição > da Apple**.</span><span class="sxs-lookup"><span data-stu-id="784ae-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens**.</span></span>

<span data-ttu-id="784ae-110">Uma das causas mais comuns de erro de sincronização é a expiração do token atual.</span><span class="sxs-lookup"><span data-stu-id="784ae-110">One of the most common causes of sync error is expiration of the current token.</span></span> <span data-ttu-id="784ae-111">Em muitos casos, a renovação do símbolo afetado resolverá a questão.</span><span class="sxs-lookup"><span data-stu-id="784ae-111">In many cases,renewal of the affected token will resolve the issue.</span></span>

<span data-ttu-id="784ae-112">Se uma ou mais das suas fichas tiver expirado, consulte a seguinte documentação para ajudá-lo a renová-las conforme apropriado:</span><span class="sxs-lookup"><span data-stu-id="784ae-112">If one or more of your tokens has expired,  see the following documentation to help you renew them as appropriate:</span></span>

[<span data-ttu-id="784ae-113">Renovar um token de inscrição de dispositivo automatizado</span><span class="sxs-lookup"><span data-stu-id="784ae-113">Renew an Automated Device Enrollment token</span></span>](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

<span data-ttu-id="784ae-114">Além disso, pode ver a seguinte documentação para ver possíveis reparações para outros erros que causam falhas de sincronização de fichas:</span><span class="sxs-lookup"><span data-stu-id="784ae-114">In addition, you can see the following documentation to see potential remediations for other errors causing token synchronization failures:</span></span>

[<span data-ttu-id="784ae-115">Erros de sincronização ABM/ASM para tokens de inscrição de dispositivos automatizados iOS/iPadOS e macOS</span><span class="sxs-lookup"><span data-stu-id="784ae-115">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[<span data-ttu-id="784ae-116">Erros de sincronização ABM/ASM para tokens de inscrição de dispositivos automatizados iOS/iPadOS e macOS</span><span class="sxs-lookup"><span data-stu-id="784ae-116">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
