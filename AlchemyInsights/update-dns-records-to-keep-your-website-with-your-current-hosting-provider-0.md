---
title: Atualizar os registos DNS para manter o seu Web site junto do seu fornecedor de alojamento atual
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 7bd36c3954d12d3ee4ac624a2f827d8e5cd88082
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665771"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="2943a-102">Atualizar os registos DNS para manter o seu Web site junto do seu fornecedor de alojamento atual</span><span class="sxs-lookup"><span data-stu-id="2943a-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="2943a-103">No centro de administração microsoft 365, vá à página De Domínios de **Configuração**  >  [Domains](https://portal.office.com/adminportal/home#/Domains) e na lista de domínios, selecione o domínio que está a utilizar para o seu website.</span><span class="sxs-lookup"><span data-stu-id="2943a-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://portal.office.com/adminportal/home#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="2943a-104">Selecione **+ Novo registo personalizado** e introduza o seguinte:</span><span class="sxs-lookup"><span data-stu-id="2943a-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="2943a-105">Para **Tipo de DNS**, introduza: **A (Endereço)**</span><span class="sxs-lookup"><span data-stu-id="2943a-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="2943a-106">Em **Nome do anfitrião ou Alias**, escreva o seguinte: **@**</span><span class="sxs-lookup"><span data-stu-id="2943a-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="2943a-107">Em **Endereço IP**, escreva o endereço IP estático onde o seu site está atualmente alojado (por exemplo, 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="2943a-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="2943a-p101">Tem de ser um endereço IP  *estático*  do site e não um endereço IP  *dinâmico*  . Verifique onde o seu site está alojado para se certificar de que consegue obter um endereço IP estático do seu site público.</span><span class="sxs-lookup"><span data-stu-id="2943a-p101">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address. Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="2943a-110">Selecione **Guardar**.</span><span class="sxs-lookup"><span data-stu-id="2943a-110">Select **Save**.</span></span>

<span data-ttu-id="2943a-111">Além disso, pode criar um registo CNAME para ajudar os clientes a encontrarem o seu site.</span><span class="sxs-lookup"><span data-stu-id="2943a-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="2943a-112">Selecione **+ Novo registo personalizado** e introduza o seguinte:</span><span class="sxs-lookup"><span data-stu-id="2943a-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="2943a-113">Para **Tipo de DNS**, introduza: **CNAME (Alias)**</span><span class="sxs-lookup"><span data-stu-id="2943a-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="2943a-114">Em **Nome do anfitrião ou Alias**, escreva o seguinte: **www**</span><span class="sxs-lookup"><span data-stu-id="2943a-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="2943a-115">Em **Aponta para o endereço**, escreva o nome de domínio completamente qualificado (FQDN) do site, (por exemplo: contoso.com</span><span class="sxs-lookup"><span data-stu-id="2943a-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="2943a-116">Selecione **Guardar**.</span><span class="sxs-lookup"><span data-stu-id="2943a-116">Select **Save**.</span></span>
