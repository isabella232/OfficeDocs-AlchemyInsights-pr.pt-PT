---
title: Alterar os Servidores de Nomes
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: 572f8befd84f55cb07a3535852a46e735d3ed620
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706766"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="4b65f-102">Atualizar os servidores de nomes do seu domínio para apontar para a Microsoft</span><span class="sxs-lookup"><span data-stu-id="4b65f-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="4b65f-103">Nota: as alterações aos servidores de nomes podem, por vezes, demorar até 48 horas a serem propagadas.</span><span class="sxs-lookup"><span data-stu-id="4b65f-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="4b65f-p101">Para configurar o seu domínio no Microsoft 365, os servidores de nomes na sua entidade de registo têm de ser atualizados. Crie ou edite os registos do seu servidor de nomes na sua entidade de registo de domínios.</span><span class="sxs-lookup"><span data-stu-id="4b65f-p101">To set up your domain in Microsoft 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="4b65f-106">Aceda ao site da sua entidade de registo de domínios e procure a área onde pode editar os servidores de nomes.</span><span class="sxs-lookup"><span data-stu-id="4b65f-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="4b65f-107">Crie ou edite dois registos de servidor de nomes de forma a que correspondam a estes valores:</span><span class="sxs-lookup"><span data-stu-id="4b65f-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="4b65f-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="4b65f-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="4b65f-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="4b65f-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="4b65f-110">Guarde as alterações.</span><span class="sxs-lookup"><span data-stu-id="4b65f-110">Save changes.</span></span>

<span data-ttu-id="4b65f-111">Também encontrará instruções detalhadas neste artigo: [Alterar servidores de nomes com qualquer entidade de registo de domínios](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="4b65f-111">You can also find detailed instructions in this article: [Change nameservers with any domain registrar](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  