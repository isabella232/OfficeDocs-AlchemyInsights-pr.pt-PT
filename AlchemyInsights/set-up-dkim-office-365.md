---
title: O programa de configuração DKIM no Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 0f81fe02135f3d0901ffe5a26d7aa3dad70c3770
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765319"
---
# <a name="setup-dkim-in-office-365"></a><span data-ttu-id="2ad2a-102">O programa de configuração DKIM no Office 365</span><span class="sxs-lookup"><span data-stu-id="2ad2a-102">Setup DKIM in Office 365</span></span>

<span data-ttu-id="2ad2a-103">As instruções completas para configurar DKIM são domínios personalizados no Office 365 [aqui](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="2ad2a-103">The complete instructions for configuring DKIM for custom domains in Office 365 are [here](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

1. <span data-ttu-id="2ad2a-104">Para **cada** domínio personalizado, tem de criar **dois** registos DKIM CNAME no serviço de alojamento do domínio DNS (normalmente, o escrivão do domínio).</span><span class="sxs-lookup"><span data-stu-id="2ad2a-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="2ad2a-105">Por exemplo, contoso.com e fourthcoffee.com requerem quatro registos DKIM CNAME: duas para contoso.com e dois para fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="2ad2a-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="2ad2a-106">Os registos DKIM CNAME para **cada** domínio personalizado, utilize os seguintes formatos:</span><span class="sxs-lookup"><span data-stu-id="2ad2a-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="2ad2a-107">**Nome de anfitrião**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="2ad2a-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="2ad2a-108">**Pontos para o endereço ou de valor**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="2ad2a-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="2ad2a-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="2ad2a-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="2ad2a-110">**Nome de anfitrião**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="2ad2a-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="2ad2a-111">**Pontos para o endereço ou de valor**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="2ad2a-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="2ad2a-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="2ad2a-112">**TTL**: 3600</span></span>

   <span data-ttu-id="2ad2a-113">\<DomainGUID\> é o texto à esquerda da `.mail.protection.outlook.com` no registo MX personalizado para o domínio personalizado (por exemplo, `contoso-com` para o domínio contoso.com).</span><span class="sxs-lookup"><span data-stu-id="2ad2a-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="2ad2a-114">\<InitialDomain\> é o domínio que utilizou quando se inscreve para Office 365 (por exemplo, contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="2ad2a-114">\<InitialDomain\> is the domain you used when you signed up for Office 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="2ad2a-115">Depois de ter criado os registos CNAME para os domínios personalizados, conclua as seguintes instruções:</span><span class="sxs-lookup"><span data-stu-id="2ad2a-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="2ad2a-116">a.</span><span class="sxs-lookup"><span data-stu-id="2ad2a-116">a.</span></span> <span data-ttu-id="2ad2a-117">[Inicie sessão no Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) com a sua conta escolar ou profissional.</span><span class="sxs-lookup"><span data-stu-id="2ad2a-117">[Sign in to Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="2ad2a-118">b.</span><span class="sxs-lookup"><span data-stu-id="2ad2a-118">b.</span></span> <span data-ttu-id="2ad2a-119">Selecione o ícone do iniciador de aplicações no canto superior esquerdo e selecione **Administrador**.</span><span class="sxs-lookup"><span data-stu-id="2ad2a-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="2ad2a-120">c.</span><span class="sxs-lookup"><span data-stu-id="2ad2a-120">c.</span></span> <span data-ttu-id="2ad2a-121">No painel de navegação no canto inferior esquerdo, expanda **Administração** e escolha o **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="2ad2a-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="2ad2a-122">d.</span><span class="sxs-lookup"><span data-stu-id="2ad2a-122">d.</span></span> <span data-ttu-id="2ad2a-123">Vá para a **protecção** > **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="2ad2a-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="2ad2a-124">e.</span><span class="sxs-lookup"><span data-stu-id="2ad2a-124">e.</span></span> <span data-ttu-id="2ad2a-125">Seleccione o domínio e, em seguida, escolher **Activar** para **mensagens de início de sessão para este domínio com assinaturas DKIM**.</span><span class="sxs-lookup"><span data-stu-id="2ad2a-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="2ad2a-126">Repita este passo para cada domínio personalizado.</span><span class="sxs-lookup"><span data-stu-id="2ad2a-126">Repeat this step for each custom domain.</span></span>
