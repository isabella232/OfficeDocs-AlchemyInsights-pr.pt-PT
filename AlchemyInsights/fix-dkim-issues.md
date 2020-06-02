---
title: Corrigir problemas de configuração DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 8195b0e3fada6da033b2d95b1fc6600e7fa3341e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506785"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="e4ea6-102">Corrigir problemas de configuração DKIM</span><span class="sxs-lookup"><span data-stu-id="e4ea6-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="e4ea6-103">Se sentir problemas que permitam ao DKIM para o seu domínio personalizado, utilize os seguintes passos:</span><span class="sxs-lookup"><span data-stu-id="e4ea6-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="e4ea6-104">A maioria dos problemas de configuração do DKIM estão relacionados com registos DNS incorretos.</span><span class="sxs-lookup"><span data-stu-id="e4ea6-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="e4ea6-105">Verifique se o registo DKIM CNAME **(não** um registo TXT) está formatado corretamente.</span><span class="sxs-lookup"><span data-stu-id="e4ea6-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="e4ea6-106">Para mais informações, consulte este [tópico.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)</span><span class="sxs-lookup"><span data-stu-id="e4ea6-106">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

- <span data-ttu-id="e4ea6-107">Depois de criar ou atualizar os registos DKIM DNS no serviço de hospedagem DNS para o seu domínio (normalmente, o seu registo de domínio), aguarde que os registos DNS se propaguem.</span><span class="sxs-lookup"><span data-stu-id="e4ea6-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="e4ea6-108">Se não conseguir criar os registos DKIM DNS no centro de administração, pode \<CustomDomain\> substituir-se pelo seu domínio personalizado (por exemplo, contoso.com) e executar este comando em [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .</span><span class="sxs-lookup"><span data-stu-id="e4ea6-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
