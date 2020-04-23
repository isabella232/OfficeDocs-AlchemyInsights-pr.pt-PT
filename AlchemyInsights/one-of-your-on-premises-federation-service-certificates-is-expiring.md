---
title: Um dos seus certificados de serviço da Federação está expirando
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: dafa344ec649002900e98a5e183b3e5f759707e1
ms.sourcegitcommit: 6a3748f5c05693ca0c19a829287cb8f30635940c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43785314"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a><span data-ttu-id="d6071-102">Um dos seus certificados de serviço da Federação está expirando</span><span class="sxs-lookup"><span data-stu-id="d6071-102">One of your on-premises Federation Service Certificates is expiring</span></span>

<span data-ttu-id="d6071-103">Para resolver esta questão, siga estes passos:</span><span class="sxs-lookup"><span data-stu-id="d6071-103">To resolve this issue, follow these steps:</span></span>
  
- <span data-ttu-id="d6071-104">Instale o Módulo de Diretório Ativo Microsoft Azure para windows PowerShell no computador (se o módulo ainda não estiver instalado).</span><span class="sxs-lookup"><span data-stu-id="d6071-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="d6071-105">Para isso, vá ao [Azure Ative Directory PowerShell para graph](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="d6071-105">To do this, go to [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span></span>
    
- <span data-ttu-id="d6071-106">Siga os passos na secção "Cenário 1: O certificado de assinatura de token AD caducou" da secção "Houve um problema de [acesso ao site" do erro da AD FS quando um utilizador federado insere na Microsoft 365, Azure ou Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="d6071-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
- <span data-ttu-id="d6071-107">Siga os passos em [Como atualizar ou reparar as definições de um domínio federado no Microsoft 365, Azure ou Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span><span class="sxs-lookup"><span data-stu-id="d6071-107">Follow the steps in [How to update or repair the settings of a federated domain in Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
<span data-ttu-id="d6071-108">Para obter mais informações sobre a renovação dos certificados da Federação, consulte a renovação do [certificado para o O365 e a AD Azure](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="d6071-108">For more information about renewing Federation certificates, see [Certificate renewal for O365 and Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
  

