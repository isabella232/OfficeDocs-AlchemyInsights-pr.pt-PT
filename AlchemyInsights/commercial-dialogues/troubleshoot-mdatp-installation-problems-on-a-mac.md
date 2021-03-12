---
title: Problemas de instalação do MDATP na resolução de problemas num Mac
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749772"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a><span data-ttu-id="ad165-102">Problemas de instalação do MDATP na resolução de problemas num Mac</span><span class="sxs-lookup"><span data-stu-id="ad165-102">Troubleshoot MDATP installation problems on a Mac</span></span>

<span data-ttu-id="ad165-103">Se a instalação manual falhar, a página **resumo** do assistente de instalação mostra o seguinte erro:</span><span class="sxs-lookup"><span data-stu-id="ad165-103">If manual installation fails, the **Summary** page of the installation wizard shows the following error:</span></span>

<span data-ttu-id="ad165-104">"Ocorreu um erro durante a instalação.</span><span class="sxs-lookup"><span data-stu-id="ad165-104">"An error occurred during installation.</span></span> <span data-ttu-id="ad165-105">O Instalador encontrou um erro que fez com que a instalação falhasse.</span><span class="sxs-lookup"><span data-stu-id="ad165-105">The Installer encountered an error that caused the installation to fail.</span></span> <span data-ttu-id="ad165-106">Contacte o fabricante de software para obter assistência."</span><span class="sxs-lookup"><span data-stu-id="ad165-106">Contact the software manufacturer for assistance."</span></span>

<span data-ttu-id="ad165-107">Para as implementações de MDM, a página também mostra uma falha genérica de instalação.</span><span class="sxs-lookup"><span data-stu-id="ad165-107">For MDM deployments, the page shows a generic installation failure, too.</span></span>

<span data-ttu-id="ad165-108">Embora não apresentemos erros exatos para os utilizadores finais, mantemos um ficheiro de registo com o progresso da instalação, em **/Library/Logs/Microsoft/mdatp/install.log**.</span><span class="sxs-lookup"><span data-stu-id="ad165-108">Although we don't display exact errors to end users, we keep a log file with installation progress, in **/Library/Logs/Microsoft/mdatp/install.log**.</span></span> <span data-ttu-id="ad165-109">Cada sessão de instalação anexa a este ficheiro de registo.</span><span class="sxs-lookup"><span data-stu-id="ad165-109">Each installation session appends to this log file.</span></span> <span data-ttu-id="ad165-110">Para obter apenas a última sessão de instalação, utilize `sed` .</span><span class="sxs-lookup"><span data-stu-id="ad165-110">To output the last installation session only, use `sed`.</span></span>

<span data-ttu-id="ad165-111">Para saber mais, consulte [problemas de instalação de resolução de problemas para o Microsoft Defender ATP para Mac](https://go.microsoft.com/fwlink/?linkid=2144615).</span><span class="sxs-lookup"><span data-stu-id="ad165-111">To learn more, see [Troubleshoot installation issues for Microsoft Defender ATP for Mac](https://go.microsoft.com/fwlink/?linkid=2144615).</span></span>
