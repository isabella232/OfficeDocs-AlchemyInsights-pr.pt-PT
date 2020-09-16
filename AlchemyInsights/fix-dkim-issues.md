---
title: Corrigir problemas de configuração DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 35e8023d26fe26211e27521ceb8751d2d7fc7a21
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744961"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="854b9-102">Corrigir problemas de configuração DKIM</span><span class="sxs-lookup"><span data-stu-id="854b9-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="854b9-103">Se sentir problemas que permitam ao DKIM para o seu domínio personalizado, utilize os seguintes passos:</span><span class="sxs-lookup"><span data-stu-id="854b9-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="854b9-104">A maioria dos problemas de configuração do DKIM estão relacionados com registos DNS incorretos.</span><span class="sxs-lookup"><span data-stu-id="854b9-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="854b9-105">Verifique se o registo DKIM CNAME **(não** um registo TXT) está formatado corretamente.</span><span class="sxs-lookup"><span data-stu-id="854b9-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="854b9-106">Para mais informações, consulte este [tópico.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)</span><span class="sxs-lookup"><span data-stu-id="854b9-106">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

- <span data-ttu-id="854b9-107">Depois de criar ou atualizar os registos DKIM DNS no serviço de hospedagem DNS para o seu domínio (normalmente, o seu registo de domínio), aguarde que os registos DNS se propaguem.</span><span class="sxs-lookup"><span data-stu-id="854b9-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="854b9-108">Se não conseguir criar os registos DKIM DNS no centro de administração, pode \<CustomDomain\> substituir-se pelo seu domínio personalizado (por exemplo, contoso.com) e executar este comando em [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .</span><span class="sxs-lookup"><span data-stu-id="854b9-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
