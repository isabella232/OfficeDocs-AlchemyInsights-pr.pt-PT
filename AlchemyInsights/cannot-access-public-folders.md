---
title: Não pode aceder a pastas públicas
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: a579b89b68bfb8432adfe64b155803eda2c3b086
ms.sourcegitcommit: a3b42ee05224846327d353b48a8c67dab724f6eb
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/21/2020
ms.locfileid: "42891760"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="8ce91-102">O Outlook não pode ligar-se a pastas públicas</span><span class="sxs-lookup"><span data-stu-id="8ce91-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="8ce91-103">Se o acesso a pasta pública não estiver a funcionar para alguns utilizadores, tente o seguinte:</span><span class="sxs-lookup"><span data-stu-id="8ce91-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="8ce91-104">Ligue-se ao EXO PowerShell e configure o parâmetro DefaultPublicFolderMailbox na conta de utilizador problemática para combinar o parâmetro numa conta de utilizador em funcionamento.</span><span class="sxs-lookup"><span data-stu-id="8ce91-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="8ce91-105">Exemplo:</span><span class="sxs-lookup"><span data-stu-id="8ce91-105">Example:</span></span>

<span data-ttu-id="8ce91-106">Caixa de correio de caixa de correio funcionador [ User] ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="8ce91-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="8ce91-107">Problemas de caixa de correio de \<conjuntoUser -DefaultPublicFolderMailbox valor de comando anterior></span><span class="sxs-lookup"><span data-stu-id="8ce91-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="8ce91-108">Espere pelo menos uma hora para que a mudança faça efeito.</span><span class="sxs-lookup"><span data-stu-id="8ce91-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="8ce91-109">Se o problema se mantiver, siga [este procedimento](https://aka.ms/pfcte) para resolver problemas de acesso a pastas públicas utilizando o Outlook.</span><span class="sxs-lookup"><span data-stu-id="8ce91-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>