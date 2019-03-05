---
title: Alterar NameServers
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: d011531a-0951-49c0-af30-40d2e765f381
ms.openlocfilehash: 61c4c5e43a247679bf18fd3861dd98fbe9a7b3eb
ms.sourcegitcommit: f1c96fd3890d4e211f7d6bf73b9105fdaab2e11c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/05/2019
ms.locfileid: "30405334"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="e8b9b-102">Atualizar os servidores de nomes do seu domínio para o Office 365</span><span class="sxs-lookup"><span data-stu-id="e8b9b-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="e8b9b-103">Nota: As alterações de servidor de nomes, por vezes, podem demorar até 48 horas para propagar.</span><span class="sxs-lookup"><span data-stu-id="e8b9b-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="e8b9b-p101">Para configurar o seu domínio no Office 365, os servidores de nomes na sua entidade de registo têm de ser atualizados. Crie ou edite os registos do seu servidor de nomes na sua entidade de registo de domínios.</span><span class="sxs-lookup"><span data-stu-id="e8b9b-p101">To set up your domain in Office 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="e8b9b-106">Aceda ao site da sua entidade de registo de domínios e procure a área onde pode editar os servidores de nomes.</span><span class="sxs-lookup"><span data-stu-id="e8b9b-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
    
2. <span data-ttu-id="e8b9b-107">Crie ou edite dois registos de servidor de nomes de forma a que correspondam a estes valores:</span><span class="sxs-lookup"><span data-stu-id="e8b9b-107">Create or edit two nameserver records to match these values:</span></span>
    
  - <span data-ttu-id="e8b9b-108">ns1.BDM.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="e8b9b-108">ns1.bdm.microsoftonline.com</span></span>
    
  - <span data-ttu-id="e8b9b-109">ns2.BDM.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="e8b9b-109">ns2.bdm.microsoftonline.com</span></span>
    
3. <span data-ttu-id="e8b9b-110">Guarde as alterações.</span><span class="sxs-lookup"><span data-stu-id="e8b9b-110">Save changes.</span></span>
    
<span data-ttu-id="e8b9b-111">Também encontrará instruções detalhadas neste artigo: [Alterar servidores de nomes para configurar o Office 365 com qualquer entidade de registo de domínios](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span><span class="sxs-lookup"><span data-stu-id="e8b9b-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span></span>
  

