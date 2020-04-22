---
title: Localização de dados
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: c769c17796d805f88afb4d5b32adb7d4a9bb3ce0
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/21/2020
ms.locfileid: "43655293"
---
# <a name="data-location"></a><span data-ttu-id="817ed-102">Localização de dados</span><span class="sxs-lookup"><span data-stu-id="817ed-102">Data location</span></span>

<span data-ttu-id="817ed-103">Pode ver a localização do seu inquilino no centro de administração ou ligando-se ao Exchange Online via PowerShell.</span><span class="sxs-lookup"><span data-stu-id="817ed-103">You can view the location of your tenant in the admin center or by connecting to Exchange Online via PowerShell.</span></span>


<span data-ttu-id="817ed-104">**Centro de administração:**</span><span class="sxs-lookup"><span data-stu-id="817ed-104">**Admin center:**</span></span>
1. <span data-ttu-id="817ed-105">Faça login no [centro de administração](https://admin.microsoft.com/Adminportal/Home).</span><span class="sxs-lookup"><span data-stu-id="817ed-105">Log in to the [admin center](https://admin.microsoft.com/Adminportal/Home).</span></span>
2. <span data-ttu-id="817ed-106">Selecione o perfil da**Organização** **de Definições** > .</span><span class="sxs-lookup"><span data-stu-id="817ed-106">Select **Settings** > **Organization profile**.</span></span>
3. <span data-ttu-id="817ed-107">Em **termos de localização de Dados,** selecione Ver **detalhes**.</span><span class="sxs-lookup"><span data-stu-id="817ed-107">Under **Data location**, select **View details**.</span></span>


<span data-ttu-id="817ed-108">**PowerShell:**</span><span class="sxs-lookup"><span data-stu-id="817ed-108">**PowerShell:**</span></span>
1. <span data-ttu-id="817ed-109">Ligue-se ao Exchange Online utilizando o Windows PowerShell.</span><span class="sxs-lookup"><span data-stu-id="817ed-109">Connect to Exchange Online by using Windows PowerShell.</span></span>
2. <span data-ttu-id="817ed-110">Execute o cmdlet [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) para apresentar uma lista das propriedades do seu inquilino.</span><span class="sxs-lookup"><span data-stu-id="817ed-110">Execute the [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet to display a list of your tenant's properties.</span></span> 
3. <span data-ttu-id="817ed-111">Olhe para a propriedade OrganizationId.</span><span class="sxs-lookup"><span data-stu-id="817ed-111">Look at the OrganizationId property.</span></span>

<span data-ttu-id="817ed-112">Quando tiver a localização dos dados para EXO e SPO, pode determinar a localização dos dados para outros serviços que poderá utilizar a partir de [onde os seus dados estão localizados](https://products.office.com/where-is-your-data-located).</span><span class="sxs-lookup"><span data-stu-id="817ed-112">When you have the data location for EXO and SPO, you can determine the data location for other services you may use from [Where your data is located](https://products.office.com/where-is-your-data-located).</span></span>