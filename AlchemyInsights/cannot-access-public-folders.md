---
title: Não é possível acessar pastas públicas
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
ms.openlocfilehash: a9305b175e1ca0b992c014a73705447d67e037bc
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959505"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="8d2c9-102">O Outlook não pode se conectar a pastas públicas</span><span class="sxs-lookup"><span data-stu-id="8d2c9-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="8d2c9-103">Se o acesso público da pasta não está funcionando para poucos usuários, tente o seguinte:</span><span class="sxs-lookup"><span data-stu-id="8d2c9-103">If public folder access isn't working for few users, try the following:</span></span>

<span data-ttu-id="8d2c9-104">Conecte-se ao EXO PowerShell e configure o DefaultPublicFolderMailbox na conta do usuário do problema para combinar uma em uma conta de usuário que trabalha.</span><span class="sxs-lookup"><span data-stu-id="8d2c9-104">Connect to EXO PowerShell, and configure the DefaultPublicFolderMailbox on the problem user account to match one on a working user account.</span></span>

<span data-ttu-id="8d2c9-105">Exemplo:</span><span class="sxs-lookup"><span data-stu-id="8d2c9-105">Example:</span></span>

<span data-ttu-id="8d2c9-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="8d2c9-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="8d2c9-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<valor de comando anterior></span><span class="sxs-lookup"><span data-stu-id="8d2c9-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="8d2c9-108">Espere pelo menos uma hora para que a mudança entre em vigor.</span><span class="sxs-lookup"><span data-stu-id="8d2c9-108">Wait at least one hour for the change to take effect.</span></span>