---
title: Trabalhar com aplicações iOS VPP Regra Id 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 67800b261e7d670181b17783bc81e276d75026e0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688957"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="255c2-102">Trabalhar com aplicações iOS VPP</span><span class="sxs-lookup"><span data-stu-id="255c2-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="255c2-103">Leia [Como gerir as aplicações iOS adquiridas através de um programa de compra de volume com o Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) para aprender sobre funcionalidades, constrangimentos e passos para utilizar o Apple Volume Purchase Program e o suporte para o mesmo no Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="255c2-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="255c2-104">**Questões comuns:** "Atribuí uma aplicação de VPP iOS aos meus utilizadores, mas a instalação falhou."</span><span class="sxs-lookup"><span data-stu-id="255c2-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="255c2-105">Isto pode acontecer se um único token VPP for usado em vários fornecedores de gestão de dispositivos móveis.</span><span class="sxs-lookup"><span data-stu-id="255c2-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="255c2-106">Os tokens VPP da Apple só podem ser usados com um fornecedor.</span><span class="sxs-lookup"><span data-stu-id="255c2-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="255c2-107">Se usou um token VPP com vários fornecedores, deve re-carregar o token para Intune.</span><span class="sxs-lookup"><span data-stu-id="255c2-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="255c2-108">A instalação também pode falhar se o número total de instalações exceder o número de licenças.</span><span class="sxs-lookup"><span data-stu-id="255c2-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="255c2-109">Para ver um relatório de utilização das suas licenças, aceda à página de licenças da Aplicação de **aplicações Intune Mobile.** \> **App licenses**</span><span class="sxs-lookup"><span data-stu-id="255c2-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="255c2-110">Para aprender a recuperar licenças em uso, consulte [este artigo.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="255c2-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
