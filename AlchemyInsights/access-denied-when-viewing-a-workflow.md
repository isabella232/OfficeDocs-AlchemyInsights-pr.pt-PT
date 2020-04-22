---
title: Acesso negado ao ver um Fluxo de Trabalho
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: c576bf88225582f2577e0b59506a7482cf9f38d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687341"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="c56ad-102">Acesso negado ao ver um Fluxo de Trabalho</span><span class="sxs-lookup"><span data-stu-id="c56ad-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="c56ad-103">O SharePoint 2013 Workflows que tentam enviar um e-mail para um grupo SharePoint pode falhar com uma mensagem de erro "Access Denied" se a adesão ao grupo SharePoint não estiver definida para todos.</span><span class="sxs-lookup"><span data-stu-id="c56ad-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="c56ad-104">**Para resolver esta questão, faça estes passos:**</span><span class="sxs-lookup"><span data-stu-id="c56ad-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="c56ad-105">Permita que todos vejam os membros do grupo SharePoint.</span><span class="sxs-lookup"><span data-stu-id="c56ad-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="c56ad-106">Remova o grupo SharePoint da linha To ou CC do e-mail.</span><span class="sxs-lookup"><span data-stu-id="c56ad-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="c56ad-107">Adicione explicitamente os utilizadores à linha To ou CC se a visibilidade da adesão não puder ser alterada para o grupo SharePoint.</span><span class="sxs-lookup"><span data-stu-id="c56ad-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="c56ad-108">Para ver mais detalhes consulte [http Unauthorized para /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="c56ad-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  