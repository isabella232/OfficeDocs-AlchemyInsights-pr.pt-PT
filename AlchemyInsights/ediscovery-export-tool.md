---
title: ferramenta de exportação eDiscovery
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: 67e59182a5053111a08f5fb2be814931a1aa815d
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277935"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a><span data-ttu-id="9e4cb-102">Não pode instalar ou executar a ferramenta de exportação eDiscovery?</span><span class="sxs-lookup"><span data-stu-id="9e4cb-102">Can't install or run the eDiscovery Export Tool?</span></span>

<span data-ttu-id="9e4cb-103">Se não conseguir instalar ou executar a Ferramenta de Exportação de eDiscovery para descarregar os resultados da pesquisa, verifique as seguintes coisas:</span><span class="sxs-lookup"><span data-stu-id="9e4cb-103">If you can't install or run the eDiscovery Export Tool to download search results, check the following things:</span></span>
  
- <span data-ttu-id="9e4cb-104">O computador que está a usar cumpre estes requisitos:</span><span class="sxs-lookup"><span data-stu-id="9e4cb-104">The computer you're using meets these pre-requisites:</span></span>

  - <span data-ttu-id="9e4cb-105">Versões de 32 ou 64 bits do Windows 7 e versões posteriores</span><span class="sxs-lookup"><span data-stu-id="9e4cb-105">32- or 64-bit versions of Windows 7 and later versions</span></span>

  - <span data-ttu-id="9e4cb-106">Microsoft .NET Framework 4.7</span><span class="sxs-lookup"><span data-stu-id="9e4cb-106">Microsoft .NET Framework 4.7</span></span>

  - <span data-ttu-id="9e4cb-107">Um navegador suportado:</span><span class="sxs-lookup"><span data-stu-id="9e4cb-107">A supported browser:</span></span>

  - <span data-ttu-id="9e4cb-108">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="9e4cb-108">Microsoft Edge</span></span>

    <span data-ttu-id="9e4cb-109">Ou</span><span class="sxs-lookup"><span data-stu-id="9e4cb-109">Or</span></span>

  - <span data-ttu-id="9e4cb-110">Versões 10 e posteriores do Internet Explorer</span><span class="sxs-lookup"><span data-stu-id="9e4cb-110">Internet Explorer 10 and later versions</span></span>

    <span data-ttu-id="9e4cb-111">Outros navegadores, como o Google Chrome e Mozilla Firefox, não são suportados.</span><span class="sxs-lookup"><span data-stu-id="9e4cb-111">Other browsers, such as Google Chrome and Mozilla Firefox aren't supported.</span></span>

- <span data-ttu-id="9e4cb-112">A sua organização pode ligar-se ao ponto final em Azure, que é \*\* \* .blob.core.windows.net\*\* (o wildcard representa um identificador único para o seu trabalho de exportação).</span><span class="sxs-lookup"><span data-stu-id="9e4cb-112">Your organization can connect to the endpoint in Azure, which is **\*.blob.core.windows.net** (the wildcard represents a unique identifier for your export job).</span></span>

- <span data-ttu-id="9e4cb-113">Foi-lhe atribuída a função de Exportação no Microsoft 365 Security &amp; Compliance Center.</span><span class="sxs-lookup"><span data-stu-id="9e4cb-113">You're assigned the Export role in the Microsoft 365 Security &amp; Compliance Center.</span></span> <span data-ttu-id="9e4cb-114">Por padrão, esta função é atribuída apenas ao grupo de funções eDiscovery Manager.</span><span class="sxs-lookup"><span data-stu-id="9e4cb-114">By default, this role is only assigned to the eDiscovery Manager role group.</span></span> <span data-ttu-id="9e4cb-115">Ver [Atribuir permissões eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span><span class="sxs-lookup"><span data-stu-id="9e4cb-115">See [Assign eDiscovery permissions](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span></span>

<span data-ttu-id="9e4cb-116">Para obter mais informações, consulte [os resultados da Pesquisa de Conteúdos de Exportação.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)</span><span class="sxs-lookup"><span data-stu-id="9e4cb-116">For more information, see [Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>

<span data-ttu-id="9e4cb-117">Se estiver a exportar mais de 100mil caixas de correio, terá de utilizar o seguinte Powershell para descarregar os resultados [da Exportação: Exportar resultados de mais de 100mil caixas de correio.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)</span><span class="sxs-lookup"><span data-stu-id="9e4cb-117">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>