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
ms.openlocfilehash: ec8fb91dfe77cb251579ce23eb0579b114b101d9
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627857"
---
# <a name="data-location"></a><span data-ttu-id="f0854-102">Localização de dados</span><span class="sxs-lookup"><span data-stu-id="f0854-102">Data location</span></span>

<span data-ttu-id="f0854-103">Você pode visualizar a localização do seu inquilino do Office 365 no centro de administração ou conectando-se ao Exchange Online via PowerShell.</span><span class="sxs-lookup"><span data-stu-id="f0854-103">You can view the location of your Office 365 tenant in the admin center or by connecting to Exchange Online via PowerShell.</span></span>


<span data-ttu-id="f0854-104">**Centro de administração:**</span><span class="sxs-lookup"><span data-stu-id="f0854-104">**Admin center:**</span></span>
1. <span data-ttu-id="f0854-105">Faça login no [centro de administração.](https://admin.microsoft.com/Adminportal/Home)</span><span class="sxs-lookup"><span data-stu-id="f0854-105">Log in to the [admin center](https://admin.microsoft.com/Adminportal/Home).</span></span>
2. <span data-ttu-id="f0854-106">Selecione o perfil da**Organização**de **Configurações** > .</span><span class="sxs-lookup"><span data-stu-id="f0854-106">Select **Settings** > **Organization profile**.</span></span>
3. <span data-ttu-id="f0854-107">De acordo com **a localização**dos dados, selecione **detalhes de exibição.**</span><span class="sxs-lookup"><span data-stu-id="f0854-107">Under **Data location**, select **View details**.</span></span>


<span data-ttu-id="f0854-108">**Powershell:**</span><span class="sxs-lookup"><span data-stu-id="f0854-108">**PowerShell:**</span></span>
1. <span data-ttu-id="f0854-109">Conecte-se ao Intercâmbio On-line usando o Windows PowerShell.</span><span class="sxs-lookup"><span data-stu-id="f0854-109">Connect to Exchange Online by using Windows PowerShell.</span></span>
2. <span data-ttu-id="f0854-110">Execute o cmdlet [get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) para exibir uma lista de propriedades do seu inquilino.</span><span class="sxs-lookup"><span data-stu-id="f0854-110">Execute the [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet to display a list of your tenant’s properties.</span></span> 
3. <span data-ttu-id="f0854-111">Olhe para a propriedade OrganizationId.</span><span class="sxs-lookup"><span data-stu-id="f0854-111">Look at the OrganizationId property.</span></span>

<span data-ttu-id="f0854-112">Quando você tem o local de dados para EXO e SPO, você pode determinar a localização dos dados para outros serviços que você pode usar [de onde seus dados estão localizados.](https://products.office.com/where-is-your-data-located)</span><span class="sxs-lookup"><span data-stu-id="f0854-112">When you have the data location for EXO and SPO, you can determine the data location for other services you may use from [Where your data is located](https://products.office.com/where-is-your-data-located).</span></span>