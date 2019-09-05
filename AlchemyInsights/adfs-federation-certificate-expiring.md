---
title: Federação ADFS certificado expirar
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
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/04/2019
ms.locfileid: "36737200"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="db4fc-102">Federação ADFS certificado expirar</span><span class="sxs-lookup"><span data-stu-id="db4fc-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="db4fc-103">Para resolver este problema, siga estes passos:</span><span class="sxs-lookup"><span data-stu-id="db4fc-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="db4fc-104">Instale o Microsoft Azure Active Directory módulo para o Windows PowerShell no computador (se o módulo já não estiver instalado).</span><span class="sxs-lookup"><span data-stu-id="db4fc-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="db4fc-105">Para efectuar este procedimento, vá para [Gerir os AD Azure utilizando o Windows PowerShell](https://aka.ms/aadposh).</span><span class="sxs-lookup"><span data-stu-id="db4fc-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="db4fc-106">Siga os passos das "cenário 1: O certificado de assinatura de tokens do AD FS expirado" secção de [erro "Ocorreu um problema ao aceder ao site" do AD FS quando um utilizador federado inicia sessão no Office 365, Azure ou Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="db4fc-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="db4fc-107">Siga os passos no [actualização ou reparar as definições de um domínio federada no Office 365, Azure ou Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span><span class="sxs-lookup"><span data-stu-id="db4fc-107">Follow the steps in [Update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span></span>

    <span data-ttu-id="db4fc-108">Para mais informações sobre como renovar certificados de Federação, consulte [renovar certificados de Federação para o Office 365 e Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="db4fc-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Office 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
