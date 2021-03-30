---
title: EndPoint Manager - Linhas de base de segurança
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
ms.openlocfilehash: d2a063fdc4929cbee5fef71bfb47ace8f2ba458f
ms.sourcegitcommit: 430d247cb5dd5dc5d1f82d977456558dfd514277
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/29/2021
ms.locfileid: "51421087"
---
# <a name="endpoint-manager---security-baselines"></a><span data-ttu-id="0c30c-102">EndPoint Manager - Linhas de base de segurança</span><span class="sxs-lookup"><span data-stu-id="0c30c-102">EndPoint Manager - Security baselines</span></span>

<span data-ttu-id="0c30c-103">As linhas de base de segurança são grupos pré-configurados de definições do Windows que o ajudam a aplicar as definições de segurança recomendadas pelas equipas de segurança relevantes.</span><span class="sxs-lookup"><span data-stu-id="0c30c-103">Security baselines are pre-configured groups of Windows settings that help you apply the security settings recommended by the relevant security teams.</span></span> <span data-ttu-id="0c30c-104">Estas linhas de base podem ser personalizadas para fornecer apenas as configurações e valores desejados.</span><span class="sxs-lookup"><span data-stu-id="0c30c-104">These baselines can be customized to deliver only the settings and values desired.</span></span> <span data-ttu-id="0c30c-105">Para obter mais informações sobre linhas de segurança, consulte [utilize linhas de base de segurança para configurar dispositivos Windows 10 no Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span><span class="sxs-lookup"><span data-stu-id="0c30c-105">For more information about security baselines, see [Use security baselines to configure Windows 10 devices in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span></span>

<span data-ttu-id="0c30c-106">Existem atualmente linhas de base para estes produtos:</span><span class="sxs-lookup"><span data-stu-id="0c30c-106">There are currently baselines for these products:</span></span>

- <span data-ttu-id="0c30c-107">Definições de segurança DO Windows MDM</span><span class="sxs-lookup"><span data-stu-id="0c30c-107">Windows MDM Security settings</span></span>
- <span data-ttu-id="0c30c-108">Microsoft Defender para Segurança EndPoint</span><span class="sxs-lookup"><span data-stu-id="0c30c-108">Microsoft Defender for EndPoint Security</span></span>
- <span data-ttu-id="0c30c-109">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="0c30c-109">Microsoft Edge</span></span>

<span data-ttu-id="0c30c-110">Cada uma das linhas de base é atualizada periodicamente e lançada em versões incrementais.</span><span class="sxs-lookup"><span data-stu-id="0c30c-110">Each of the baselines are updated periodically and released in incremental versions.</span></span> <span data-ttu-id="0c30c-111">Cada versão adiciona e remove as definições da versão anterior para garantir que a linha de base satisfaz a orientação atual.</span><span class="sxs-lookup"><span data-stu-id="0c30c-111">Each version adds and or removes settings from the previous version to ensure that the baseline meets current guidance.</span></span> <span data-ttu-id="0c30c-112">A consola de bases de segurança em Endpoint Security permite comparar diferentes versões, tornando visíveis as alterações da versão para a versão.</span><span class="sxs-lookup"><span data-stu-id="0c30c-112">The Security baselines console in Endpoint Security allows different versions to be compared by making the changes from version to version visible.</span></span>

<span data-ttu-id="0c30c-113">Para obter orientações sobre como alterar de forma mais eficaz qual a versão de linha de base implementada, consulte [Gerir os perfis de base de segurança no Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span><span class="sxs-lookup"><span data-stu-id="0c30c-113">For guidance on how to most effectively change which version of baseline is deployed, see [Manage security baseline profiles in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span></span>

<span data-ttu-id="0c30c-114">Depois de implementar uma linha de base de segurança, pode monitorizar o estado de implementação e revisão das definições numa base dispositivo por dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0c30c-114">After deploying a security baseline, you can monitor the state of deployment and review settings on a device-by-device basis.</span></span>

<span data-ttu-id="0c30c-115">**Nota:** Os dados de reporte das linhas de base podem demorar até 24 horas a aparecer desde a implantação inicial a um dispositivo e até 6 horas para novas atualizações.</span><span class="sxs-lookup"><span data-stu-id="0c30c-115">**Note:** The reporting data for baselines may take up to 24 hours to appear from the initial deployment to a device and up to 6 hours for further updates.</span></span> 

<span data-ttu-id="0c30c-116">A causa mais comum de uma definição de linha de base não aplicada é porque a mesma definição está sendo usada num perfil diferente.</span><span class="sxs-lookup"><span data-stu-id="0c30c-116">The most common cause of a baseline setting not applying is because the same setting being used in a different profile.</span></span> <span data-ttu-id="0c30c-117">Este cenário pode ser investigado para dispositivos específicos selecionando esse dispositivo a partir do nó de Estado do Dispositivo do perfil base de segurança.</span><span class="sxs-lookup"><span data-stu-id="0c30c-117">This scenario can be investigated for specific device by selecting that device from within the Device Status node of the Security Baseline profile.</span></span> <span data-ttu-id="0c30c-118">Para mais detalhes, consulte [resolver conflitos para linhas de base de segurança](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span><span class="sxs-lookup"><span data-stu-id="0c30c-118">For details, see [Resolve conflicts for security baselines](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span></span>