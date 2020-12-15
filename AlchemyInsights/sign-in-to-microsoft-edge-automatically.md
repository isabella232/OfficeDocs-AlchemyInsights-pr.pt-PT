---
title: Iniciar sôms automaticamente no Microsoft Edge
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
ms.openlocfilehash: 68a1119abd0a3f687b6448bb6e58c6485c239c0f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678812"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a><span data-ttu-id="db895-102">Iniciar sôms automaticamente no Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="db895-102">Sign in to Microsoft Edge automatically</span></span>

<span data-ttu-id="db895-103">O Microsoft Edge utiliza a conta predefinida do SISTEMA para assinar automaticamente num utilizador de acordo com a configuração do dispositivo do utilizador.</span><span class="sxs-lookup"><span data-stu-id="db895-103">Microsoft Edge uses the OS's default account to automatically sign in a user according to how the user's device is configured.</span></span> 

<span data-ttu-id="db895-104">Os cenários de cada tipo de configuração do dispositivo e do seu processo de inscrição do utilizador dependente são descritos abaixo:</span><span class="sxs-lookup"><span data-stu-id="db895-104">The scenarios of each type of device configuration and its dependent user sign-in process are described below:</span></span>

1. <span data-ttu-id="db895-105">**O dispositivo é híbrido/AAD-J:** Esta opção está disponível no Windows 10, windows de nível inferior e versões de servidor correspondentes.</span><span class="sxs-lookup"><span data-stu-id="db895-105">**The device is hybrid/AAD-J**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="db895-106">Os utilizadores são automaticamente inscritos nas suas contas Azure Ative Directory (AD)."</span><span class="sxs-lookup"><span data-stu-id="db895-106">Users are automatically signed in with their Azure Active Directory (AD)accounts.</span></span>
2. <span data-ttu-id="db895-107">**O dispositivo está ligado ao domínio**: Esta opção está disponível no Windows 10, no Windows de nível inferior e nas versões correspondentes do servidor.</span><span class="sxs-lookup"><span data-stu-id="db895-107">**The device is domain-joined**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="db895-108">Por padrão, os utilizadores com contas de domínio não são assinados automaticamente; para permitir o seu registo automático, utilize a política **ConfigureOnPremisesAccountAutoSignIn.**</span><span class="sxs-lookup"><span data-stu-id="db895-108">By default, users with domain accounts are not signed in automatically; to enable automatic sign-in for them, use the **ConfigureOnPremisesAccountAutoSignIn** policy.</span></span> <span data-ttu-id="db895-109">Para permitir o registo automático dos utilizadores com contas AD Azure, considere a junção híbrida dos seus dispositivos.</span><span class="sxs-lookup"><span data-stu-id="db895-109">To enable automatic sign-in for users with Azure AD accounts, consider hybrid-joining their devices.</span></span>
3. <span data-ttu-id="db895-110">**A conta padrão do SISTEMA é uma conta Microsoft**: Esta opção está disponível no Windows 10 RS3 (versão 1709, construa 10.0.16299) e versões posteriores.</span><span class="sxs-lookup"><span data-stu-id="db895-110">**The OS's default account is a Microsoft account**: This option is available on Windows 10 RS3 (version 1709, build 10.0.16299) and later versions.</span></span> <span data-ttu-id="db895-111">É pouco provável que o cenário ocorra em dispositivos empresariais.</span><span class="sxs-lookup"><span data-stu-id="db895-111">The scenario is unlikely to occur on enterprise devices.</span></span> <span data-ttu-id="db895-112">No entanto, se a conta padrão do SISTEMA for uma conta Microsoft, então o Microsoft Edge assinará automaticamente no utilizador com a conta microsoft.</span><span class="sxs-lookup"><span data-stu-id="db895-112">However, if the OS's default account is a Microsoft account, then Microsoft Edge will automatically sign in the user with the Microsoft account.</span></span>
 
 
