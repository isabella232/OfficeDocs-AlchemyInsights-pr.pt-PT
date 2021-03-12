---
title: Corrigir problemas comuns com formatação de registo dKIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 0a59ca1c93121cb4681c0d44b85a9b756c07895b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750760"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a><span data-ttu-id="4a399-102">Corrigir problemas comuns com formatação de registo dKIM</span><span class="sxs-lookup"><span data-stu-id="4a399-102">Fix common problems with DKIM record formatting</span></span>

<span data-ttu-id="4a399-103">A maioria dos problemas de configuração do DKIM estão relacionados com registos DNS incorretos.</span><span class="sxs-lookup"><span data-stu-id="4a399-103">Most DKIM set-up issues are related to incorrect DNS records.</span></span>

<span data-ttu-id="4a399-104">Para corrigir os problemas de configuração do DKIM, verifique se o registo DKIM CNAME **(não** um registo TXT) está formatado corretamente.</span><span class="sxs-lookup"><span data-stu-id="4a399-104">To fix the DKIM set-up issues, verify that the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="4a399-105">Para mais informações, consulte [o que precisa de fazer para configurar manualmente o DKIM no Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).</span><span class="sxs-lookup"><span data-stu-id="4a399-105">For more information, see [What you need to do to manually set up DKIM in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).</span></span>

<span data-ttu-id="4a399-106">Se precisar de ajuda com registos DNS em geral, consulte [crie registos DNS em qualquer fornecedor de hospedagem DNS para o Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).</span><span class="sxs-lookup"><span data-stu-id="4a399-106">If you need help with DNS records in general, see [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).</span></span>

> [!NOTE]
> <span data-ttu-id="4a399-107">Depois de criar ou atualizar os seus registos DKIM DNS no serviço de hospedagem DNS para o seu domínio, terá de esperar que os registos DNS se propaguem.</span><span class="sxs-lookup"><span data-stu-id="4a399-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain, you'll need to wait for the DNS records to propagate.</span></span>
