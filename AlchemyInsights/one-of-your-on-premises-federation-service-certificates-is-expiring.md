---
title: Um dos seus certificados de serviço de federação local estiver prestes a expirar
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: 9e2e1a1dd2993b2a02b4405db8a707b23ff4af16
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/30/2019
ms.locfileid: "29658918"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a><span data-ttu-id="daf99-102">Um dos seus certificados de serviço de federação local estiver prestes a expirar</span><span class="sxs-lookup"><span data-stu-id="daf99-102">One of your on-premises Federation Service Certificates is expiring</span></span>

<span data-ttu-id="daf99-103">Para resolver este problema, siga estes passos:</span><span class="sxs-lookup"><span data-stu-id="daf99-103">To resolve this issue, follow these steps:</span></span>
  
- <span data-ttu-id="daf99-p101">Instale o Microsoft Azure Active Directory módulo para o Windows PowerShell no computador (se o módulo já não estiver instalado). Para tal, vá para [Azure Active Directory PowerShell para gráfico](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="daf99-p101">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed). To do this, go to [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span></span>
    
- <span data-ttu-id="daf99-106">Siga os passos das "cenário 1: O certificado de assinatura de tokens do AD FS expirado" secção de [erro "Ocorreu um problema ao aceder ao site" do AD FS quando um utilizador federado inicia sessão no Office 365, Azure ou Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="daf99-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
- <span data-ttu-id="daf99-107">Siga os passos no t[como actualizar ou reparar as definições de um domínio federada no Office 365, Azure ou Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span><span class="sxs-lookup"><span data-stu-id="daf99-107">Follow the steps in t[How to update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
<span data-ttu-id="daf99-108">Para mais informações sobre como renovar certificados de Federação, consulte a [renovação de certificados para O365 e Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="daf99-108">For more information about renewing Federation certificates, see [Certificate renewal for O365 and Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
  

