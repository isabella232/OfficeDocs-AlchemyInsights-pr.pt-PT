---
title: Corrigir problemas de configuração DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 4d6dadbcbf71fe6e9ea56d6a82a7d8ababdd38ef
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765307"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="231b8-102">Corrigir problemas de configuração DKIM</span><span class="sxs-lookup"><span data-stu-id="231b8-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="231b8-103">Se tiver problemas a activação de DKIM para o domínio personalizado, utilize os seguintes passos:</span><span class="sxs-lookup"><span data-stu-id="231b8-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="231b8-104">A maior parte dos problemas de configuração DKIM estão relacionados com registos DNS incorrectos.</span><span class="sxs-lookup"><span data-stu-id="231b8-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="231b8-105">Verifique se que o registo DKIM CNAME (**não** um registo TXT) está correctamente formatado.</span><span class="sxs-lookup"><span data-stu-id="231b8-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="231b8-106">Para mais informações, consulte este [tópico](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="231b8-106">For more information, see this [topic](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

- <span data-ttu-id="231b8-107">Depois de criar ou actualizar os registos de DNS de DKIM no DNS que hospeda o serviço para o domínio (normalmente, o escrivão do domínio), aguarde que os registos de DNS propagar.</span><span class="sxs-lookup"><span data-stu-id="231b8-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="231b8-108">Se não conseguir criar o DNS DKIM registos no Centro de administração, pode substituir \<CustomDomain\> com o domínio personalizado (por exemplo, contoso.com) e execute este comando no [PowerShell Online do Exchange](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span><span class="sxs-lookup"><span data-stu-id="231b8-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
