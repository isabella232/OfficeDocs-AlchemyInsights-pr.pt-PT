---
title: Configuração virtual com serviços de domínio AAD
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7927"
- "9004397"
ms.openlocfilehash: 7c56e467679f9b9a48cfd7a6f70f7ee148ded3e8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885646"
---
# <a name="virtual-configuration-with-aad-domain-services"></a><span data-ttu-id="6a40b-102">Configuração virtual com serviços de domínio AAD</span><span class="sxs-lookup"><span data-stu-id="6a40b-102">Virtual configuration with AAD domain services</span></span>

<span data-ttu-id="6a40b-103">A configuração virtual com os serviços de domínio AAD envolve os seguintes passos:</span><span class="sxs-lookup"><span data-stu-id="6a40b-103">Virtual configuration with AAD domain services involves the following steps:</span></span> 

1. <span data-ttu-id="6a40b-104">Verificar a saúde do seu domínio no portal Azure https://aka.ms/aadds-health</span><span class="sxs-lookup"><span data-stu-id="6a40b-104">Checking your domain’s health on the Azure portal https://aka.ms/aadds-health</span></span>
2. <span data-ttu-id="6a40b-105">Verificando o seu NSG por regras que bloqueiam portas necessárias para sincronizar em Azure AD Domain Services no portal https://aka.ms/aadds-networking</span><span class="sxs-lookup"><span data-stu-id="6a40b-105">Checking your NSG for rules that block ports needed to synchronize in Azure AD Domain Services on the portal https://aka.ms/aadds-networking</span></span>
3. <span data-ttu-id="6a40b-106">Certificando-se de que a sua rede virtual é implantada na mesma Região Azure que o seu domínio gerido pelos Serviços de Domínio AZure AD.</span><span class="sxs-lookup"><span data-stu-id="6a40b-106">Ensuring that your virtual network is deployed in the same Azure Region as your Azure AD Domain Services-managed domain.</span></span>
4. <span data-ttu-id="6a40b-107">Garantindo que não tem um domínio existente com o mesmo nome de domínio disponível na rede virtual.</span><span class="sxs-lookup"><span data-stu-id="6a40b-107">Ensuring you don’t have an existent domain with the same domain name available on the virtual network.</span></span>

<span data-ttu-id="6a40b-108">Para obter mais detalhes sobre a consideração de design na Rede Virtual Azure para apoiar os serviços de domínio AAD, consulte [Adyssed de Rede Virtual](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).</span><span class="sxs-lookup"><span data-stu-id="6a40b-108">For more details on design consideration on Azure Virtual Network to support AAD domain services, see [Virtual Network Consideration](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).</span></span>

