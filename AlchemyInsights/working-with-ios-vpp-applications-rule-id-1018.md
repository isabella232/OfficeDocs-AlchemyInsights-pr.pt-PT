---
title: Trabalhar com iOS VPP aplicações regra Id 1018
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 65b9a727171a7551068717f6327f15e1aa8e6bed
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32420495"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="7c959-102">Trabalhar com iOS VPP aplicações</span><span class="sxs-lookup"><span data-stu-id="7c959-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="7c959-103">Leia [como gerir aplicações de iOS adquiridas através de um programa de volume de compras com Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) para obter informações sobre funcionalidades, restrições e passos para que utilize o programa de compras de Volume da Apple e o suporte para o mesmo no Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="7c959-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span> 
  
 <span data-ttu-id="7c959-104">**Problemas comuns:** "Que atribuí uma aplicação VPP iOS a meus utilizadores, mas falha na instalação."</span><span class="sxs-lookup"><span data-stu-id="7c959-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span> 
  
- <span data-ttu-id="7c959-105">Isto pode acontecer se um token VPP único é utilizado através de vários fornecedores de gestão do dispositivo móvel.</span><span class="sxs-lookup"><span data-stu-id="7c959-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="7c959-106">Os tokens VPP de Apple só podem ser utilizados com um fornecedor.</span><span class="sxs-lookup"><span data-stu-id="7c959-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="7c959-107">Se utilizou um token VPP com vários fornecedores, tem de carregar novamente o token para Intune.</span><span class="sxs-lookup"><span data-stu-id="7c959-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>
    
- <span data-ttu-id="7c959-108">A instalação também pode falhar se o número total de instalações exceder o número de licenças.</span><span class="sxs-lookup"><span data-stu-id="7c959-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="7c959-109">Para ver um relatório de utilização para as licenças, vá para o **apps Intune Mobile** \> página de **licenças de aplicação** .</span><span class="sxs-lookup"><span data-stu-id="7c959-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="7c959-110">Para obter informações sobre como recuperar de licenças em utilização, consulte [deste artigo.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="7c959-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
    

