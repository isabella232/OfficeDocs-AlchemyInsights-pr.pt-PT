---
title: Conflitos com SourceAnchor, ProxyAddress, UserPrincipalName
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1699"
- "1300022"
ms.openlocfilehash: 826dfe9e5c7d24ff5186a94e1ada4dad536e7edd
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/20/2020
ms.locfileid: "45198570"
---
# <a name="conflicts-with-sourceanchor-proxyaddress-userprincipalname"></a><span data-ttu-id="0e667-102">Conflitos com SourceAnchor, ProxyAddress, UserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0e667-102">Conflicts with SourceAnchor, ProxyAddress, UserPrincipalName</span></span>

<span data-ttu-id="0e667-103">Se receber erros durante uma sincronização como "Um objeto sincronizado com o mesmo ProxyAddress ou UserPrincipalName existe no seu diretório", consulte [diagnóstico e remediar erros de sincronização de atributos duplicados](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-diagnose-sync-errors).</span><span class="sxs-lookup"><span data-stu-id="0e667-103">If you receive errors during a synchronization such as "A synchronized object with the same ProxyAddress or UserPrincipalName exists in your directory", see [Diagnose and remediate duplicated attribute sync errors](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-diagnose-sync-errors).</span></span>

<span data-ttu-id="0e667-104">Além disso, considere permitir a duplicação da resiliência do atributo.</span><span class="sxs-lookup"><span data-stu-id="0e667-104">Also, consider enabling duplicate attribute resiliency.</span></span> <span data-ttu-id="0e667-105">Para obter mais informações, consulte [a sincronização de identidade e duplicar a resiliência do atributo](https://aka.ms/duplicateattributeresiliency).</span><span class="sxs-lookup"><span data-stu-id="0e667-105">For more info, see [Identity synchronization and duplicate attribute resiliency](https://aka.ms/duplicateattributeresiliency).</span></span>