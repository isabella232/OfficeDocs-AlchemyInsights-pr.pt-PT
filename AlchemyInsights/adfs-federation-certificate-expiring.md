---
title: Caducidade do certificado da Federação ADFS
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 14e7da6220dfa96edca5d9ec5c32e003480a9eaf
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43710418"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="e439d-102">Caducidade do certificado da Federação ADFS</span><span class="sxs-lookup"><span data-stu-id="e439d-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="e439d-103">Para resolver esta questão, siga estes passos:</span><span class="sxs-lookup"><span data-stu-id="e439d-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="e439d-104">Instale o Módulo de Diretório Ativo Microsoft Azure para windows PowerShell no computador (se o módulo ainda não estiver instalado).</span><span class="sxs-lookup"><span data-stu-id="e439d-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="e439d-105">Para isso, vá para [a Manage Azure AD utilizando o Windows PowerShell](https://aka.ms/aadposh).</span><span class="sxs-lookup"><span data-stu-id="e439d-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="e439d-106">Siga os passos na secção "Cenário 1: O certificado de assinatura de token AD caducou" da secção "Houve um problema de [acesso ao site" do erro da AD FS quando um utilizador federado insere na Microsoft 365, Azure ou Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="e439d-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="e439d-107">Siga os passos em [Atualizar ou repare as definições de um domínio federado na Microsoft, Azure ou Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span><span class="sxs-lookup"><span data-stu-id="e439d-107">Follow the steps in [Update or repair the settings of a federated domain in Microsoft, Azure, or Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span></span>

    <span data-ttu-id="e439d-108">Para saber mais sobre a renovação dos certificados da Federação, consulte Renovar os certificados da federação para o [Microsoft 365 e o Azure Ative Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="e439d-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Microsoft 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
