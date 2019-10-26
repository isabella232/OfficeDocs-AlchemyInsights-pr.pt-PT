---
title: Certificado da Federação ADFS expirando
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: eafd31e91340b41b7948fb1fe62889731b816d9a
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/25/2019
ms.locfileid: "36737200"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="ac828-102">Certificado da Federação ADFS expirando</span><span class="sxs-lookup"><span data-stu-id="ac828-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="ac828-103">Para resolver este problema, siga estas etapas:</span><span class="sxs-lookup"><span data-stu-id="ac828-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="ac828-104">Instale o Módulo de Diretório Ativo do Microsoft Azure para Windows PowerShell no computador (se o módulo ainda não estiver instalado).</span><span class="sxs-lookup"><span data-stu-id="ac828-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="ac828-105">Para fazer isso, acesse [o AD do Azure usando o Windows PowerShell.](https://aka.ms/aadposh)</span><span class="sxs-lookup"><span data-stu-id="ac828-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="ac828-106">Siga os passos na seção "Cenário 1: O certificado de assinatura de tokens AD FS expirou" de "Houve um problema de [acesso ao site" erro de AD FS quando um usuário federado assina para o Office 365, Azure, ou Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="ac828-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="ac828-107">Siga as [etapas em Atualização ou repare as configurações de um domínio federado no Office 365, Azure ou Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span><span class="sxs-lookup"><span data-stu-id="ac828-107">Follow the steps in [Update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span></span>

    <span data-ttu-id="ac828-108">Para saber mais sobre a renovação de certificados da Federação, consulte os certificados da federação Renew para o [Office 365 e o Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)</span><span class="sxs-lookup"><span data-stu-id="ac828-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Office 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
