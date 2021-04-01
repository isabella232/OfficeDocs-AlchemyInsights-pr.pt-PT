---
title: Endpoint Manager - Linhas de base de segurança
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
- "10064"
- "9003771"
ms.openlocfilehash: 36b480c7ed4715338fda056eafd69c511093e627
ms.sourcegitcommit: bef118c00aa397cd6d8941d403fe9cfa49dd8c73
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/30/2021
ms.locfileid: "51440895"
---
# <a name="endpoint-manager---security-baselines"></a><span data-ttu-id="a733b-102">Endpoint Manager - Linhas de base de segurança</span><span class="sxs-lookup"><span data-stu-id="a733b-102">EndPoint Manager - Security baselines</span></span>

<span data-ttu-id="a733b-103">As linhas de base de segurança são grupos pré-configurados de definições do Windows que o ajudam a aplicar as definições de segurança recomendadas pelas equipas de segurança relevantes.</span><span class="sxs-lookup"><span data-stu-id="a733b-103">Security baselines are pre-configured groups of Windows settings that help you apply the security settings recommended by the relevant security teams.</span></span> <span data-ttu-id="a733b-104">Estas linhas de base podem ser personalizadas para aplicar apenas as definições e os valores pretendidos.</span><span class="sxs-lookup"><span data-stu-id="a733b-104">These baselines can be customized to deliver only the settings and values desired.</span></span> <span data-ttu-id="a733b-105">Para obter mais informações sobre as linhas de base de segurança, consulte [Utilizar linhas de base de segurança para configurar dispositivos Windows 10 no Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span><span class="sxs-lookup"><span data-stu-id="a733b-105">For more information about security baselines, see [Use security baselines to configure Windows 10 devices in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span></span>

<span data-ttu-id="a733b-106">Apenas existem linhas de base para estes produtos:</span><span class="sxs-lookup"><span data-stu-id="a733b-106">There are currently baselines for these products:</span></span>

- <span data-ttu-id="a733b-107">Definições de segurança do Windows MDM</span><span class="sxs-lookup"><span data-stu-id="a733b-107">Windows MDM Security settings</span></span>
- <span data-ttu-id="a733b-108">Segurança do Microsoft Defender para Ponto Final</span><span class="sxs-lookup"><span data-stu-id="a733b-108">Microsoft Defender for EndPoint Security</span></span>
- <span data-ttu-id="a733b-109">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="a733b-109">Microsoft Edge</span></span>

<span data-ttu-id="a733b-110">Cada uma das linhas de base é atualizada periodicamente e lançada em versões incrementais.</span><span class="sxs-lookup"><span data-stu-id="a733b-110">Each of the baselines are updated periodically and released in incremental versions.</span></span> <span data-ttu-id="a733b-111">Cada versão adiciona e/ou remove as definições da versão anterior para garantir que a linha de base cumpre as orientações atuais.</span><span class="sxs-lookup"><span data-stu-id="a733b-111">Each version adds and or removes settings from the previous version to ensure that the baseline meets current guidance.</span></span> <span data-ttu-id="a733b-112">A consola de Linhas de base de segurança no Endpoint Security permite-lhe comparar versões diferentes ao tornar visíveis as alterações de versão para versão.</span><span class="sxs-lookup"><span data-stu-id="a733b-112">The Security baselines console in Endpoint Security allows different versions to be compared by making the changes from version to version visible.</span></span>

<span data-ttu-id="a733b-113">Para obter orientações sobre a forma mais eficiente de alterar a versão da linha de base que é implementada, consulte [Gerir perfis de segurança de linha de base no Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span><span class="sxs-lookup"><span data-stu-id="a733b-113">For guidance on how to most effectively change which version of baseline is deployed, see [Manage security baseline profiles in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span></span>

<span data-ttu-id="a733b-114">Após implementar uma linha de base de segurança, pode monitorizar o estado da implementação e rever as definições dispositivo a dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a733b-114">After deploying a security baseline, you can monitor the state of deployment and review settings on a device-by-device basis.</span></span>

<span data-ttu-id="a733b-115">**Nota:** os dados de relatórios das linhas de base podem demorar até 24 horas a serem apresentados após a implementação inicial para um dispositivo, e até 6 horas para atualizações futuras.</span><span class="sxs-lookup"><span data-stu-id="a733b-115">**Note:** The reporting data for baselines may take up to 24 hours to appear from the initial deployment to a device and up to 6 hours for further updates.</span></span> 

<span data-ttu-id="a733b-116">A causa mais comum de uma definição de linha de base não ser aplicada prende-se com o facto de a mesma definição estar a ser utilizada num perfil diferente.</span><span class="sxs-lookup"><span data-stu-id="a733b-116">The most common cause of a baseline setting not applying is because the same setting being used in a different profile.</span></span> <span data-ttu-id="a733b-117">Este cenário pode ser investigado num dispositivo específico, ao selecionar o mesmo a partir do nó do Estado do Dispositivo do perfil de Linha de Base de segurança.</span><span class="sxs-lookup"><span data-stu-id="a733b-117">This scenario can be investigated for specific device by selecting that device from within the Device Status node of the Security Baseline profile.</span></span> <span data-ttu-id="a733b-118">Para obter detalhes, consulte [Resolver conflitos de linhas de base de segurança](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span><span class="sxs-lookup"><span data-stu-id="a733b-118">For details, see [Resolve conflicts for security baselines](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span></span>