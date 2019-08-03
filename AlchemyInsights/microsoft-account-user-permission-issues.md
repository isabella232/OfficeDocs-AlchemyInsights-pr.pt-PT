---
title: Resolver a questão - o utilizador não encontrado no directório
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 0909edc581c811fdc4683b004e0df0adbac88d1c
ms.sourcegitcommit: 514ced512d0d7fff485b6fbf236cd27d6b4166e0
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/26/2019
ms.locfileid: "35249924"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="f5b0f-102">Resolver a questão - o utilizador não encontrado no directório</span><span class="sxs-lookup"><span data-stu-id="f5b0f-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="f5b0f-103">Se os utilizadores estão a receber erros mensagem "utilizador não é possível localizar" no directório.</span><span class="sxs-lookup"><span data-stu-id="f5b0f-103">If users are receiving error message "user can't be found" in the directory.</span></span> <span data-ttu-id="f5b0f-104">Tente novamente quando o tipo de problema utilizador não estiver no directório.</span><span class="sxs-lookup"><span data-stu-id="f5b0f-104">Please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="f5b0f-105">Os seguintes passos podem ser concluídos para resolver o problema.</span><span class="sxs-lookup"><span data-stu-id="f5b0f-105">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="f5b0f-106">Certifique-se a conta que aceite que o convite de correio electrónico é a mesma conta que está a ser utilizada para iniciar sessão mais tarde.</span><span class="sxs-lookup"><span data-stu-id="f5b0f-106">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="f5b0f-107">Certifique-se do que utilizador está a utilizar a mesma conta para a aceitar o convite e iniciar sessão no site.</span><span class="sxs-lookup"><span data-stu-id="f5b0f-107">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="f5b0f-108">Para obter mais informações, consulte [como gerir aliases para sua conta Microsoft</a> para gerir o início de sessão do Office 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="f5b0f-108">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="f5b0f-109">Navegue para cada site em que o utilizador está a receber o erro.</span><span class="sxs-lookup"><span data-stu-id="f5b0f-109">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="f5b0f-110">Adicionar "/ _layouts/15/people.aspx/membershipgroupid=0" (entre as aspas) para o fim do URL do site.</span><span class="sxs-lookup"><span data-stu-id="f5b0f-110">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="f5b0f-111">Exemplo: https://_lT _"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="f5b0f-111">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="f5b0f-112">Seleccione o utilizador a partir da lista.</span><span class="sxs-lookup"><span data-stu-id="f5b0f-112">Select the user from the list.</span></span>

- <span data-ttu-id="f5b0f-113">Clique em **remover permissões de utilizador** do Friso.</span><span class="sxs-lookup"><span data-stu-id="f5b0f-113">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="f5b0f-114">Voltar a adicionar o utilizador e reenvie o convite para o utilizador.</span><span class="sxs-lookup"><span data-stu-id="f5b0f-114">Add back the User and Resend the invite to the user.</span></span>

