---
title: Acesso negado ao visualizar um fluxo de trabalho
ms.author: pebaum
author: pebaum
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 1cfda8e08ada05858a28f2bede8c31261f9de351
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050536"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="d8daf-102">Acesso negado ao visualizar um fluxo de trabalho</span><span class="sxs-lookup"><span data-stu-id="d8daf-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="d8daf-103">Fluxos de trabalho do SharePoint 2013 que tentam enviar um e-mail para um grupo SharePoint podem falhar com uma mensagem de erro "Access Denied" se a associação do grupo SharePoint não for definida para todos.</span><span class="sxs-lookup"><span data-stu-id="d8daf-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="d8daf-104">**Para resolver esse problema, faça essas etapas:**</span><span class="sxs-lookup"><span data-stu-id="d8daf-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="d8daf-105">Permita que todos vejam os membros do grupo SharePoint.</span><span class="sxs-lookup"><span data-stu-id="d8daf-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="d8daf-106">Retire o grupo SharePoint da linha To ou CC do e-mail.</span><span class="sxs-lookup"><span data-stu-id="d8daf-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="d8daf-107">Adicione explicitamente os usuários à linha To ou CC se a visibilidade da associação não puder ser alterada para o grupo SharePoint.</span><span class="sxs-lookup"><span data-stu-id="d8daf-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="d8daf-108">Para ver mais detalhes, consulte HTTP [Não autorizado a /_vti_bin/client.svc/sp.utilities.utility.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="d8daf-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  