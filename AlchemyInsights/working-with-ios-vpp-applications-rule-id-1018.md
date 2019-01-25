---
title: Trabalhar com iOS VPP aplicações regra Id 1018
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 5bcfb6dd7222bd102ff2620c19bfb943e7bd9591
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/24/2019
ms.locfileid: "29484237"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="9d5dc-102">Trabalhar com iOS VPP aplicações</span><span class="sxs-lookup"><span data-stu-id="9d5dc-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="9d5dc-103">Leia [como gerir aplicações de iOS adquiridas através de um programa de volume de compras com Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) para obter informações sobre funcionalidades, restrições e passos para que utilize o programa de compras de Volume da Apple e o suporte para o mesmo no Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="9d5dc-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span> 
  
 <span data-ttu-id="9d5dc-104">**Problemas comuns:** "Que atribuí uma aplicação VPP iOS a meus utilizadores, mas falha na instalação."</span><span class="sxs-lookup"><span data-stu-id="9d5dc-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span> 
  
- <span data-ttu-id="9d5dc-p101">Isto pode acontecer se um token VPP único é utilizado através de vários fornecedores de gestão do dispositivo móvel. Os tokens VPP de Apple só podem ser utilizados com um fornecedor. Se utilizou um token VPP com vários fornecedores, tem de carregar novamente o token para Intune.</span><span class="sxs-lookup"><span data-stu-id="9d5dc-p101">This can happen if a single VPP token is used across multiple mobile device management providers. VPP tokens from Apple may only be used with one provider. If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>
    
- <span data-ttu-id="9d5dc-p102">A instalação também pode falhar se o número total de instalações exceder o número de licenças. Para ver um relatório de utilização para as licenças, vá para o **apps Intune Mobile** \> página de **licenças de aplicação** . Para obter informações sobre como recuperar de licenças em utilização, consulte [deste artigo.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="9d5dc-p102">The installation can also fail if the total number of installations exceed the number of licenses. To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page. To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
    

