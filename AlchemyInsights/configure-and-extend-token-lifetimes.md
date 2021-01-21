---
title: Configurar e prolongar as vidas simbólicas
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: 505e79ae9a163b89a6df2a7085480728bb0f1051
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/20/2021
ms.locfileid: "49917008"
---
# <a name="configure-and-extend-token-lifetimes"></a><span data-ttu-id="bc2ed-102">Configurar e prolongar as vidas simbólicas</span><span class="sxs-lookup"><span data-stu-id="bc2ed-102">Configure and extend token lifetimes</span></span>

<span data-ttu-id="bc2ed-103">Pode especificar o tempo de vida útil de um token de acesso, SAML ou ID emitido pela plataforma de identidade Microsoft.</span><span class="sxs-lookup"><span data-stu-id="bc2ed-103">You can specify the lifetime of an access, SAML, or ID token issued by Microsoft identity platform.</span></span> <span data-ttu-id="bc2ed-104">Você pode definir vidas simbólicas para todas as aplicações da sua organização, para uma aplicação multi-inquilina (multi-organização) ou para um diretor de serviço específico na sua organização.</span><span class="sxs-lookup"><span data-stu-id="bc2ed-104">You can set token lifetimes for all apps in your organization, for a multi-tenant (multi-organization) application, or for a specific service principal in your organization.</span></span> <span data-ttu-id="bc2ed-105">Para mais informações, leia [as vidas simbólicas configuráveis.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)</span><span class="sxs-lookup"><span data-stu-id="bc2ed-105">For more info, read [configurable token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

<span data-ttu-id="bc2ed-106">Por exemplo, leia [exemplos de como configurar vidas simbólicas.](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes)</span><span class="sxs-lookup"><span data-stu-id="bc2ed-106">For examples, read [examples of how to configure token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).</span></span>

<span data-ttu-id="bc2ed-107">Para aprender a configurar a vida e a compatibilidade de um símbolo em Azure Ative Directory B2C (Azure AD B2C), consulte [fichas de configuração no Azure Ative Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).</span><span class="sxs-lookup"><span data-stu-id="bc2ed-107">To learn how to configure the lifetime and compatibility of a token in Azure Active Directory B2C (Azure AD B2C), see [Configure tokens in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).</span></span>

<span data-ttu-id="bc2ed-108">O artigo [Configurar o comportamento da sessão no Azure Ative Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) descreve os métodos de assinatura única (SSO) utilizados no Azure AD B2C e ajuda-o a escolher o método SSO mais adequado ao configurar a sua política.</span><span class="sxs-lookup"><span data-stu-id="bc2ed-108">The article [Configure session behavior in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) describes the single sign-on (SSO) methods used in Azure AD B2C and helps you choose the most appropriate SSO method when configuring your policy.</span></span>

<span data-ttu-id="bc2ed-109">**Quanto tempo duram as fichas? Por quanto tempo são válidos?**</span><span class="sxs-lookup"><span data-stu-id="bc2ed-109">**How long do tokens last? How long are they valid for?**</span></span>

<span data-ttu-id="bc2ed-110">As vidas simbólicas são de 1 hora e a vida útil da sessão é de 24 horas.</span><span class="sxs-lookup"><span data-stu-id="bc2ed-110">Token lifetimes are 1 hour and the session lifetime is 24 hours.</span></span> <span data-ttu-id="bc2ed-111">Isto significa que, se não houver pedidos em 24 horas, terá de fazer login novamente antes de pedir um novo token.</span><span class="sxs-lookup"><span data-stu-id="bc2ed-111">This means that if no requests have been made in 24 hours, you will need to log in again before requesting a new token.</span></span>

> [!NOTE]
> <span data-ttu-id="bc2ed-112">Depois de 30 de maio de 2020, nenhum novo inquilino poderá usar a política de Vida Token Configurada para configurar sessão e refrescar tokens.</span><span class="sxs-lookup"><span data-stu-id="bc2ed-112">After May 30, 2020, no new tenant will be able to use Configurable Token Lifetime policy to configure session and refresh tokens.</span></span> <span data-ttu-id="bc2ed-113">A depreciação acontecerá dentro de alguns meses, o que significa que deixaremos de honrar a sessão existente e refrescaremos as polícias.</span><span class="sxs-lookup"><span data-stu-id="bc2ed-113">The deprecation will happen within several months after that, which means that we will stop honoring existing session and refresh tokens polices.</span></span> <span data-ttu-id="bc2ed-114">Ainda pode configurar o acesso a vidas simbólicas após a depreciação.</span><span class="sxs-lookup"><span data-stu-id="bc2ed-114">You can still configure access token lifetimes after the deprecation.</span></span>






