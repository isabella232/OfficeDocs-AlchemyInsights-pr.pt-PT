---
title: Fazer descoberta do site
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9143"
- "9005291"
ms.openlocfilehash: bdf94220de45d92f63e56501ea4e35389224d25c
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694561"
---
# <a name="do-site-discovery"></a><span data-ttu-id="7df33-102">Fazer descoberta do site</span><span class="sxs-lookup"><span data-stu-id="7df33-102">Do site discovery</span></span>

<span data-ttu-id="7df33-103">Se a sua organização ainda usa aplicações web antigas e planeia usar o modo Internet Explorer (o que a maioria dos clientes usa), então deve fazer alguma descoberta adicional do site.</span><span class="sxs-lookup"><span data-stu-id="7df33-103">If your organization still uses legacy web applications and plans to use Internet Explorer mode (which most customers do), then you should do some additional site discovery.</span></span>

<span data-ttu-id="7df33-104">**Já implementou uma versão mais antiga do Microsoft Edge**</span><span class="sxs-lookup"><span data-stu-id="7df33-104">**You've already deployed an older version of Microsoft Edge**</span></span>

<span data-ttu-id="7df33-105">Se já configuraste a tua Lista de Sites da Empresa para trabalhares para a versão antiga do Microsoft Edge, então a descoberta do teu site está quase pronta.</span><span class="sxs-lookup"><span data-stu-id="7df33-105">If you've already configured your Enterprise Site List to work for the legacy version of Microsoft Edge, then your site discovery is almost done.</span></span> <span data-ttu-id="7df33-106">A única coisa que talvez precises de fazer é adicionar sítios neutros.</span><span class="sxs-lookup"><span data-stu-id="7df33-106">The one thing you might need to do is add neutral sites.</span></span>

<span data-ttu-id="7df33-107">Os locais neutros são normalmente sites que fornecem um único sinal de inscrição (SSO).</span><span class="sxs-lookup"><span data-stu-id="7df33-107">Neutral sites are typically sites that provide single sign-on (SSO).</span></span> <span data-ttu-id="7df33-108">Se for a um site neutro do Microsoft Edge, então pretende ficar no Microsoft Edge para autenticar.</span><span class="sxs-lookup"><span data-stu-id="7df33-108">If you go to a neutral site from Microsoft Edge, then you want to stay in Microsoft Edge to authenticate.</span></span> <span data-ttu-id="7df33-109">Se for a um site neutro no modo Internet Explorer, então deseja permanecer no modo Internet Explorer para autenticar.</span><span class="sxs-lookup"><span data-stu-id="7df33-109">If you go to a neutral site in Internet Explorer mode, then you want to stay in Internet Explorer mode to authenticate.</span></span>

<span data-ttu-id="7df33-110">Identifique quaisquer SSO ou outros sites neutros que utilize e adicione-os à sua Lista de Site Empresarial.</span><span class="sxs-lookup"><span data-stu-id="7df33-110">Identify any SSO or other neutral sites that you use and add these to your Enterprise Site List.</span></span>

<span data-ttu-id="7df33-111">**O Internet Explorer é o seu navegador padrão**</span><span class="sxs-lookup"><span data-stu-id="7df33-111">**Internet Explorer is your default browser**</span></span>

<span data-ttu-id="7df33-112">Se você só está usando o Internet Explorer agora, você pode não saber quais sites atualizaram para padrões web modernos e que ainda requerem Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="7df33-112">If you're only using Internet Explorer now, you might not know which sites have upgraded to modern web standards and which still require Internet Explorer.</span></span> <span data-ttu-id="7df33-113">Você vai querer encontrar e adicionar estes sites à Lista de Sites da Empresa para que possa usar o modo Internet Explorer apenas para esses sites.</span><span class="sxs-lookup"><span data-stu-id="7df33-113">You'll want to find and add these sites to the Enterprise Site List so that you can use Internet Explorer mode only for those sites.</span></span>

> [!NOTE]
> <span data-ttu-id="7df33-114">[Enterprise Site Discovery](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) descobre sites que podem necessitar do modo Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="7df33-114">[Enterprise Site Discovery](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) discovers sites that might need Internet Explorer mode.</span></span> <span data-ttu-id="7df33-115">Pode recolher dados em computadores que executam o Windows Internet Explorer 8 através do Internet Explorer 11 no Windows 10, Windows 8.1 ou Windows 7.</span><span class="sxs-lookup"><span data-stu-id="7df33-115">It can collect data on computers running Windows Internet Explorer 8 through Internet Explorer 11 on Windows 10, Windows 8.1, or Windows 7.</span></span>

<span data-ttu-id="7df33-116">**Analisar os dados**</span><span class="sxs-lookup"><span data-stu-id="7df33-116">**Analyze the data**</span></span>

<span data-ttu-id="7df33-117">Depois de recolher os dados do site, recomendamos o seguinte processo de quatro etapas para analisar os dados:</span><span class="sxs-lookup"><span data-stu-id="7df33-117">After you've collected site data, we recommend the following four-step process to analyze the data:</span></span>
1. <span data-ttu-id="7df33-118">Ordenar os dados por domínio e, em seguida, por URL.</span><span class="sxs-lookup"><span data-stu-id="7df33-118">Sort the data by domain, and then by URL.</span></span>
2. <span data-ttu-id="7df33-119">Defina os limites de uma aplicação para configurar para o modo Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="7df33-119">Define the boundaries of an app to configure for Internet Explorer mode.</span></span> <span data-ttu-id="7df33-120">Pretende incluir todos os sites e controlos web que definem a aplicação, mas não quer incluir sites e controlos extras.</span><span class="sxs-lookup"><span data-stu-id="7df33-120">You want to include all the sites and web controls that define the app, but you don't want to include extra sites and controls.</span></span> <span data-ttu-id="7df33-121">Alguns sites podem ser tão simples como *https://contoso.com/app1* outros podem exigir que você defina vários sites e páginas.</span><span class="sxs-lookup"><span data-stu-id="7df33-121">Some sites might be as simple as *https://contoso.com/app1* while others might require you to define multiple sites and pages.</span></span>
3. <span data-ttu-id="7df33-122">Teste a aplicação para verificar se não funciona de forma nativa.</span><span class="sxs-lookup"><span data-stu-id="7df33-122">Test the app to verify that it doesn't work natively.</span></span> <span data-ttu-id="7df33-123">Muitos sites oferecem conteúdo moderno quando detetam um navegador moderno e só oferecem conteúdo legado quando detetam o Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="7df33-123">Many sites will offer modern content when they detect a modern browser and only offer legacy content when they detect Internet Explorer.</span></span>
4. <span data-ttu-id="7df33-124">Adicione a aplicação à sua Lista de Sites da Empresa se falhar no teste.</span><span class="sxs-lookup"><span data-stu-id="7df33-124">Add the app to your Enterprise Site List if it fails testing.</span></span>

> [!NOTE]
> <span data-ttu-id="7df33-125">Como uma boa prática, agrupem todos os sites que compõem uma aplicação.</span><span class="sxs-lookup"><span data-stu-id="7df33-125">As a best practice, group all of the sites that comprise an app.</span></span> <span data-ttu-id="7df33-126">Desta forma, quando atualiza uma aplicação, é mais fácil remover todo o site do modo Internet Explorer e começar a usar um navegador moderno para essa aplicação.</span><span class="sxs-lookup"><span data-stu-id="7df33-126">This way, when you upgrade an app, it's easier to remove the entire site from Internet Explorer mode and start using a modern browser for that app.</span></span>

<span data-ttu-id="7df33-127">Assim que terminar a descoberta do site e analisar os dados, está pronto para começar a olhar para a sua estratégia de canal.</span><span class="sxs-lookup"><span data-stu-id="7df33-127">Once you're done with site discovery and you've analyzed the data, you're ready to start looking at your channel strategy.</span></span>

