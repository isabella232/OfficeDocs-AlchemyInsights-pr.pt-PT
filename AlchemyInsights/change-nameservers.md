---
title: Alterar os Servidores de Nomes
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: 51532f42e7cbd39ebad3f0160465218c6e1454a2
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/04/2019
ms.locfileid: "36736660"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="73633-102">Atualizar os servidores de nomes do seu domínio para o Office 365</span><span class="sxs-lookup"><span data-stu-id="73633-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="73633-103">Nota: as alterações aos servidores de nomes podem, por vezes, demorar até 48 horas a serem propagadas.</span><span class="sxs-lookup"><span data-stu-id="73633-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="73633-p101">Para configurar o seu domínio no Office 365, os servidores de nomes na sua entidade de registo têm de ser atualizados. Crie ou edite os registos do seu servidor de nomes na sua entidade de registo de domínios.</span><span class="sxs-lookup"><span data-stu-id="73633-p101">To set up your domain in Office 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="73633-106">Aceda ao site da sua entidade de registo de domínios e procure a área onde pode editar os servidores de nomes.</span><span class="sxs-lookup"><span data-stu-id="73633-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="73633-107">Crie ou edite dois registos de servidor de nomes de forma a que correspondam a estes valores:</span><span class="sxs-lookup"><span data-stu-id="73633-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="73633-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="73633-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="73633-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="73633-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="73633-110">Guarde as alterações.</span><span class="sxs-lookup"><span data-stu-id="73633-110">Save changes.</span></span>

<span data-ttu-id="73633-111">Também encontrará instruções detalhadas neste artigo: [Alterar servidores de nomes para configurar o Office 365 com qualquer entidade de registo de domínios](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="73633-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  