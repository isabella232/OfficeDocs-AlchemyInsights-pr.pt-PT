---
title: Trabalhar com aplicações iOS VPP Regra Id 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 88a1ef66bf337b3a0094976c122330591aee77ff
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43719968"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="911c6-102">Trabalhar com aplicações iOS VPP</span><span class="sxs-lookup"><span data-stu-id="911c6-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="911c6-103">Leia [como gerir as aplicações iOS adquiridas através de um programa de compra de volume com](https://docs.microsoft.com/intune/vpp-apps-ios) o Microsoft Intune para aprender sobre funcionalidades, constrangimentos e passos para fazer uso do Programa de Compra de Volume apple e o suporte para o mesmo no Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="911c6-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="911c6-104">**Questões Comuns:** "Atribuí uma aplicação iOS VPP aos meus utilizadores, mas a instalação falhou."</span><span class="sxs-lookup"><span data-stu-id="911c6-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="911c6-105">Isto pode acontecer se um único token VPP for usado em vários fornecedores de gestão de dispositivos móveis.</span><span class="sxs-lookup"><span data-stu-id="911c6-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="911c6-106">Os tokens VPP da Apple só podem ser usados com um fornecedor.</span><span class="sxs-lookup"><span data-stu-id="911c6-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="911c6-107">Se usou um símbolo VPP com vários fornecedores, tem de voltar a carregar o token para Intune.</span><span class="sxs-lookup"><span data-stu-id="911c6-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="911c6-108">A instalação também pode falhar se o número total de instalações exceder o número de licenças.</span><span class="sxs-lookup"><span data-stu-id="911c6-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="911c6-109">Para ver um relatório de utilização das suas licenças, vá à página de **licenças** de \> **aplicações Intune Mobile.**</span><span class="sxs-lookup"><span data-stu-id="911c6-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="911c6-110">Para aprender a recuperar licenças em uso, consulte [este artigo.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="911c6-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
