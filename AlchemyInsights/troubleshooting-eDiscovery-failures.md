---
title: 1490-resolução de problemas-falhas na descoberta
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1490"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: ff28f96d64ec14980e9a47b630246b394faf4610
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277845"
---
# <a name="troubleshoot-content-search-errors"></a><span data-ttu-id="475cc-102">Resolução de problemas Erros de pesquisa de conteúdo</span><span class="sxs-lookup"><span data-stu-id="475cc-102">Troubleshoot Content Search errors</span></span>

<span data-ttu-id="475cc-103">Está a ter problemas com a Pesquisa de Conteúdo ou com falhas quando exporta resultados de pesquisa?</span><span class="sxs-lookup"><span data-stu-id="475cc-103">Are you experiencing problems with Content Search or getting failures when you export search results?</span></span>

<span data-ttu-id="475cc-104">Por exemplo, está a receber o seguinte ao fazer pesquisas?</span><span class="sxs-lookup"><span data-stu-id="475cc-104">For example, are you receiving the following when running searches?</span></span>

- <span data-ttu-id="475cc-105">Erros CS008 ou CS012</span><span class="sxs-lookup"><span data-stu-id="475cc-105">CS008 or CS012 errors</span></span>

- <span data-ttu-id="475cc-106">Erros ocupados/tempoout do servidor</span><span class="sxs-lookup"><span data-stu-id="475cc-106">Server busy/timeout errors</span></span>

- <span data-ttu-id="475cc-107">Erro de aplicação ocorreu</span><span class="sxs-lookup"><span data-stu-id="475cc-107">Application error occurred</span></span>

<span data-ttu-id="475cc-108">Ou quando pesquisar ou exportar resulta de um grande número de caixas de correio (mais de 100.000 caixas de correio), está a obter erros de exportação?</span><span class="sxs-lookup"><span data-stu-id="475cc-108">Or when searching or exporting results from a large number of mailboxes (over 100,000 mailboxes), are you getting export errors?</span></span>

<span data-ttu-id="475cc-109">Para este tipo de erros, recandiduça a procura das localizações de conteúdo que falharam.</span><span class="sxs-lookup"><span data-stu-id="475cc-109">For these types of errors, retry the search for the content locations that have failed.</span></span> <span data-ttu-id="475cc-110">Consulte  [este artigo](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) para mais informações.</span><span class="sxs-lookup"><span data-stu-id="475cc-110">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>

<span data-ttu-id="475cc-111">Se estiver a exportar mais de 100mil caixas de correio, terá de utilizar o seguinte Powershell para descarregar os resultados [da Exportação: Exportar resultados de mais de 100mil caixas de correio.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)</span><span class="sxs-lookup"><span data-stu-id="475cc-111">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>
