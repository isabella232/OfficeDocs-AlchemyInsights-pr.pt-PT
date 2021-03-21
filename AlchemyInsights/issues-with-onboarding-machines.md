---
title: Problemas com a inclusão de computadores no Microsoft Defender para Ponto Final
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 7ccec69f8ab43f277978176519a7f8f8df443846
ms.sourcegitcommit: 1d73771d147325cfd8578e6816becd8331913890
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/19/2021
ms.locfileid: "50901578"
---
# <a name="issues-with-onboarding-machines-to-microsoft-defender-for-endpoints"></a><span data-ttu-id="2edb9-102">Problemas com a inclusão de computadores no Microsoft Defender para Ponto Final</span><span class="sxs-lookup"><span data-stu-id="2edb9-102">Issues with onboarding machines to Microsoft Defender for Endpoints</span></span>

<span data-ttu-id="2edb9-103">Poderá ter problemas com a inclusão de computadores com o serviço MDE.</span><span class="sxs-lookup"><span data-stu-id="2edb9-103">You might have issues with onboarding machines to MDE service.</span></span> <span data-ttu-id="2edb9-104">Se consegue aceder ao computador do utilizador final, siga estes passos:</span><span class="sxs-lookup"><span data-stu-id="2edb9-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="2edb9-105">Transfira a versão de pré-visualização da ferramenta de diagnóstico [MDE Client Analyzer](https://aka.ms/betamdeanalyzer).</span><span class="sxs-lookup"><span data-stu-id="2edb9-105">Download the latest preview version of the [MDE Client Analyzer](https://aka.ms/betamdeanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="2edb9-106">Clique com o botão direito do rato em **MDEClientAnalyzer.cmd** e selecione "Executar como administrador".</span><span class="sxs-lookup"><span data-stu-id="2edb9-106">Right click **MDEClientAnalyzer.cmd** and select ‘Run as administrator’.</span></span>
3. <span data-ttu-id="2edb9-107">Siga as orientações sugeridas em **MDEClientAnalyzer.htm**.</span><span class="sxs-lookup"><span data-stu-id="2edb9-107">Follow any guidance suggested in **MDEClientAnalyzer.htm**.</span></span>
4. <span data-ttu-id="2edb9-108">Para obter registos mais detalhados, consulte a subpasta criada com o nome **MDEClientAnalyzerResult**.</span><span class="sxs-lookup"><span data-stu-id="2edb9-108">For more verbose logs, review the created sub-folder named **MDEClientAnalyzerResult**.</span></span>
5. <span data-ttu-id="2edb9-109">Se necessitar de orientações adicionais, contacte o [suporte do Microsoft Defender para Ponto Final](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) e forneça o ficheiro MDEClientAnalyzerResult.zip resultante para análise.</span><span class="sxs-lookup"><span data-stu-id="2edb9-109">If additional guidance is needed, contact [Microsoft Defender for Endpoint support](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) and provide the resulting MDEClientAnalyzerResult.zip file for analysis.</span></span>
