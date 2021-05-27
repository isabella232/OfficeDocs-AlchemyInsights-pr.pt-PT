---
title: Regras de redução da superfície de ataque
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11228"
- "9005470"
ms.openlocfilehash: 99feaa5c3f35a0bb78b99f47ac2be88cf3e1b62a
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676439"
---
# <a name="attack-surface-reduction-rules"></a><span data-ttu-id="ea850-102">Regras de redução da superfície de ataque</span><span class="sxs-lookup"><span data-stu-id="ea850-102">Attack surface reduction rules</span></span>

<span data-ttu-id="ea850-103">Excluir ficheiros ou pastas pode reduzir gravemente a proteção fornecida pelas regras de redução da superfície de ataque.</span><span class="sxs-lookup"><span data-stu-id="ea850-103">Excluding files or folders can severely reduce the protection provided by attack surface reduction rules.</span></span> <span data-ttu-id="ea850-104">Os ficheiros que teriam sido bloqueados por uma regra têm permissão para ser executados e não é registado nenhum relatório ou evento.</span><span class="sxs-lookup"><span data-stu-id="ea850-104">Files that would have been blocked by a rule are allowed to run, and no report or event is recorded.</span></span> <span data-ttu-id="ea850-105">Uma exclusão aplica-se a todas as regras que permitem exclusões.</span><span class="sxs-lookup"><span data-stu-id="ea850-105">An exclusion applies to all rules that allow exclusions.</span></span>

<span data-ttu-id="ea850-106">As exclusões ASR utilizam a mesma sintaxe que as Antivírus do Microsoft Defender exclusões.</span><span class="sxs-lookup"><span data-stu-id="ea850-106">ASR exclusions use the same syntax as Microsoft Defender Antivirus exclusions.</span></span> <span data-ttu-id="ea850-107">Para obter detalhes, [consulte Configurar e validar exclusões para Antivírus do Microsoft Defender análises.](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="ea850-107">For details, see [Configure and validate exclusions for Microsoft Defender Antivirus scans](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus).</span></span> <span data-ttu-id="ea850-108">Para evitar problemas, [reveja erros comuns a evitar ao definir exclusões](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="ea850-108">To avoid problems, review [Common mistakes to avoid when defining exclusions](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="ea850-109">Nem todas as regras ASR suportam exclusões.</span><span class="sxs-lookup"><span data-stu-id="ea850-109">Not all ASR rules support exclusions.</span></span> <span data-ttu-id="ea850-110">Para validar se a sua regra suporta exclusões, consulte a tabela Regras de redução da [superfície de ataque](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span><span class="sxs-lookup"><span data-stu-id="ea850-110">To validate if your rule supports exclusions, see the table [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

## <a name="attack-surface-reduction-rules"></a><span data-ttu-id="ea850-111">Regras de redução da superfície de ataque</span><span class="sxs-lookup"><span data-stu-id="ea850-111">Attack surface reduction rules</span></span>

<span data-ttu-id="ea850-112">A superfície de ataque da sua organização inclui todos os locais onde um atacante pode comprometer os dispositivos ou redes da organização.</span><span class="sxs-lookup"><span data-stu-id="ea850-112">Your organization attack surface includes all the places where an attacker could compromise organization devices or networks.</span></span> <span data-ttu-id="ea850-113">Reduzir a sua superfície de ataque significa proteger os dispositivos e a rede da organização, o que deixa os atacantes com menos formas de efetuar ataques.</span><span class="sxs-lookup"><span data-stu-id="ea850-113">Reducing your attack surface means protecting the organization devices and network, which leaves attackers with fewer ways to perform attacks.</span></span> <span data-ttu-id="ea850-114">Configurar regras de redução da superfície de ataque no Microsoft Defender para Pontos Finais pode ajudar.</span><span class="sxs-lookup"><span data-stu-id="ea850-114">Configuring attack surface reduction rules in Microsoft Defender for Endpoint can help.</span></span>

<span data-ttu-id="ea850-115">Para mais informações, consulte:</span><span class="sxs-lookup"><span data-stu-id="ea850-115">For more information, see:</span></span>

- [<span data-ttu-id="ea850-116">Mapear GUID da regra ASR para nome</span><span class="sxs-lookup"><span data-stu-id="ea850-116">Map ASR rule GUID to name</span></span>](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- <span data-ttu-id="ea850-117">Requisitos de regras ASR:</span><span class="sxs-lookup"><span data-stu-id="ea850-117">ASR rules requirements:</span></span>
    - [<span data-ttu-id="ea850-118">Windows 10 Pro, versão 1709 ou posterior</span><span class="sxs-lookup"><span data-stu-id="ea850-118">Windows 10 Pro, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="ea850-119">Windows 10 Enterprise, versão 1709 ou posterior</span><span class="sxs-lookup"><span data-stu-id="ea850-119">Windows 10 Enterprise, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="ea850-120">Windows Servidor, versão 1803 (Via de Atualizações Semesuais) ou posterior</span><span class="sxs-lookup"><span data-stu-id="ea850-120">Windows Server, version 1803 (Semi-Annual Channel) or later</span></span>](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a><span data-ttu-id="ea850-121">Identificar a exclusão correta a aplicar</span><span class="sxs-lookup"><span data-stu-id="ea850-121">Identify the correct exclusion to apply</span></span>

1. <span data-ttu-id="ea850-122">Procure o eventID 1121 ou 1122 no registo Microsoft-Windows-Windows Defender/Operacional.</span><span class="sxs-lookup"><span data-stu-id="ea850-122">Look for eventID 1121 or 1122 in the Microsoft-Windows-Windows Defender/Operational log.</span></span>

1. <span data-ttu-id="ea850-123">Avalie o cenário e o contexto do bloqueio e confirme que este cenário tem de ser desbloqueado.</span><span class="sxs-lookup"><span data-stu-id="ea850-123">Evaluate the block scenario and context and confirm that this scenario needs to be unblocked.</span></span>

1. <span data-ttu-id="ea850-124">Leia o valor Caminho nos detalhes do evento, que é o valor que define a exclusão.</span><span class="sxs-lookup"><span data-stu-id="ea850-124">Read the Path value in the event details, which is the value that defines the exclusion.</span></span>
    - <span data-ttu-id="ea850-125">Tornar a exclusão o mais estrita possível.</span><span class="sxs-lookup"><span data-stu-id="ea850-125">Make the exclusion as strict as possible.</span></span>
    - <span data-ttu-id="ea850-126">Aplicar um cartão wildcard onde for necessário (por exemplo, substituir variável de Utilizador).</span><span class="sxs-lookup"><span data-stu-id="ea850-126">Apply a wildcard where needed (for example, replace User variable).</span></span>

1. <span data-ttu-id="ea850-127">Aplique a exclusão de acordo com as suas necessidades de implementação.</span><span class="sxs-lookup"><span data-stu-id="ea850-127">Apply the exclusion according to your deployment needs.</span></span> <span data-ttu-id="ea850-128">Para obter detalhes, consulte [Personalizar regras de redução da superfície de ataque](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).</span><span class="sxs-lookup"><span data-stu-id="ea850-128">For details, see [Customize attack surface reduction rules](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).</span></span>

## <a name="exclusion-is-not-honored"></a><span data-ttu-id="ea850-129">A exclusão não é honrada</span><span class="sxs-lookup"><span data-stu-id="ea850-129">Exclusion is not honored</span></span>

1. <span data-ttu-id="ea850-130">Determine se a regra suporta exclusões.</span><span class="sxs-lookup"><span data-stu-id="ea850-130">Determine whether the rule support exclusions.</span></span> <span data-ttu-id="ea850-131">Para obter detalhes, consulte Regras de redução [da superfície de ataque](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span><span class="sxs-lookup"><span data-stu-id="ea850-131">For details, see [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

1. <span data-ttu-id="ea850-132">Reveja as exclusões aplicadas e verifique com os dados do evento se existem erros tipográficos ou comnados.</span><span class="sxs-lookup"><span data-stu-id="ea850-132">Review the exclusions applied and verify with the event data for typos or misinterpreted wildcards.</span></span> <span data-ttu-id="ea850-133">Para mais informações, consulte Tipos de [exclusão suportados](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span><span class="sxs-lookup"><span data-stu-id="ea850-133">For more info, see [Supported exclusion types](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span></span>

1. <span data-ttu-id="ea850-134">se o impacto da regra for demasiado elevado, considere mover a regra (para trás) para o Modo de auditoria para efetuar uma validação posterior.</span><span class="sxs-lookup"><span data-stu-id="ea850-134">if the impact of the rule it too high, consider moving the rule (back) to Audit mode to perform further validation.</span></span> <span data-ttu-id="ea850-135">Para obter detalhes, consulte [Testar como o Microsoft Defender para funcionalidades do Endpoint funciona em modo de auditoria.](/microsoft-365/security/defender-endpoint/audit-windows-defender)</span><span class="sxs-lookup"><span data-stu-id="ea850-135">For details, see [Test how Microsoft Defender for Endpoint features work in audit mode](/microsoft-365/security/defender-endpoint/audit-windows-defender).</span></span>

1. <span data-ttu-id="ea850-136">Recolha dados de suporte para abrir um caso de suporte utilizando este comando:</span><span class="sxs-lookup"><span data-stu-id="ea850-136">Collect support data to open a support case by using this command:</span></span>
    
   <span data-ttu-id="ea850-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span><span class="sxs-lookup"><span data-stu-id="ea850-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span></span>

    <span data-ttu-id="ea850-138">Para obter mais informações, consulte [Problemas com os sistemas de iboarding no Microsoft Defender para Pontos finais.](issues-with-onboarding-machines.md)</span><span class="sxs-lookup"><span data-stu-id="ea850-138">For more information, see [Issues with onboarding machines to Microsoft Defender for Endpoints](issues-with-onboarding-machines.md).</span></span>
