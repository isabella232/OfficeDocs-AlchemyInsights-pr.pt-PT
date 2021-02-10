---
title: Implementar AD FS
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1300012"
- "7420"
ms.openlocfilehash: a304504f7483036884878639dfa6ebfc3cdfcac8
ms.sourcegitcommit: 05a9dd3121c21322dc9ddec4c2eec548cafd5a43
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177720"
---
# <a name="deploy-ad-fs"></a><span data-ttu-id="1d53b-102">Implementar AD FS</span><span class="sxs-lookup"><span data-stu-id="1d53b-102">Deploy AD FS</span></span>

<span data-ttu-id="1d53b-103">Uma implantação de Serviços da Federação de Diretórios Ativos (AD FS) utiliza a sua infraestrutura no local para autenticar os utilizadores para os serviços do Office 365.</span><span class="sxs-lookup"><span data-stu-id="1d53b-103">An Active Directory Federation Services (AD FS) deployment uses your on-premises infrastructure to authenticate users for ‎Office 365 services.</span></span> <span data-ttu-id="1d53b-104">Com o registo federado, pode permitir que os utilizadores inscrevam-se nos serviços e software do Office 365 como um Serviço (SAAS) que estão integrados com o Azure Ative Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="1d53b-104">With federated sign-in, you can enable users to sign in to Office 365 services and Software as a Service (SAAS) applications that are integrated with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="1d53b-105">O sign-in federado autentica os utilizadores contra o seu Ative Directy no local via AD FS.</span><span class="sxs-lookup"><span data-stu-id="1d53b-105">Federated sign-in authenticates users against your on-premises Active Directory via AD FS.</span></span> <span data-ttu-id="1d53b-106">Além disso, enquanto estiver na rede corporativa, os utilizadores não serão obrigados a reentrar nas suas palavras-passe.</span><span class="sxs-lookup"><span data-stu-id="1d53b-106">Also, while on the corporate network, users won't be required to reenter their passwords.</span></span>

<span data-ttu-id="1d53b-107">O [consultor de implementação AD FS](https://go.microsoft.com/fwlink/?linkid=2071178) fornece-lhe orientações passo a passo sobre a implementação de uma infraestrutura AD FS no local que autentica os utilizadores para os serviços Microsoft 365 e Office 365.</span><span class="sxs-lookup"><span data-stu-id="1d53b-107">The [AD FS deployment advisor](https://go.microsoft.com/fwlink/?linkid=2071178) provides you with step-by-step guidance on deploying an on-premises AD FS infrastructure that authenticates users for Microsoft 365 and Office 365 services.</span></span> <span data-ttu-id="1d53b-108">Com este guia, a sua organização pode rever componentes e requisitos AD FS, adquirir e instalar certificados SSL necessários para a implementação e instalar um servidor de procuração de aplicações web necessários.</span><span class="sxs-lookup"><span data-stu-id="1d53b-108">With this guide, your organization can review AD FS components and requirements, acquire and install SSL certificates that are necessary for deployment, and install a required web application proxy server.</span></span>
