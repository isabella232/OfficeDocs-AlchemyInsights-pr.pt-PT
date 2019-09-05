---
title: Atualizar os servidores de nomes do seu domínio para o Office 365
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 5/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 23d49c734148739ede0d5e5b53430a42b606c831
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/04/2019
ms.locfileid: "36742195"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="2900c-102">Atualizar os servidores de nomes do seu domínio para o Office 365</span><span class="sxs-lookup"><span data-stu-id="2900c-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="2900c-103">Nota: as alterações aos servidores de nomes podem, por vezes, demorar até 48 horas a serem propagadas.</span><span class="sxs-lookup"><span data-stu-id="2900c-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="2900c-p101">Para configurar o seu domínio no Office 365, os servidores de nomes na sua entidade de registo têm de ser atualizados. Crie ou edite os registos do seu servidor de nomes na sua entidade de registo de domínios.</span><span class="sxs-lookup"><span data-stu-id="2900c-p101">To set up your domain in Office 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="2900c-106">Aceda ao site da sua entidade de registo de domínios e procure a área onde pode editar os servidores de nomes.</span><span class="sxs-lookup"><span data-stu-id="2900c-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="2900c-107">Crie ou edite dois registos de servidor de nomes de forma a que correspondam a estes valores:</span><span class="sxs-lookup"><span data-stu-id="2900c-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="2900c-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="2900c-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="2900c-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="2900c-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="2900c-110">Guarde as alterações.</span><span class="sxs-lookup"><span data-stu-id="2900c-110">Save changes.</span></span>

<span data-ttu-id="2900c-111">Também encontrará instruções detalhadas neste artigo: [Alterar servidores de nomes para configurar o Office 365 com qualquer entidade de registo de domínios](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="2900c-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  