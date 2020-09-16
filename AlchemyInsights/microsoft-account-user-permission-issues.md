---
title: Problema de resolução de problemas - Utilizador não encontrado no diretório
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 512494a69ab274af00962cb9777a3479b4200fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725418"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="a94d7-102">Problema de resolução de problemas - Utilizador não encontrado no diretório</span><span class="sxs-lookup"><span data-stu-id="a94d7-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="a94d7-103">Se os utilizadores estiverem a receber uma mensagem de erro "o utilizador não pode ser encontrado" no diretório, tente novamente onde o Tipo de Problemas está no diretório do Utilizador.</span><span class="sxs-lookup"><span data-stu-id="a94d7-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="a94d7-104">Os seguintes passos podem ser concluídos para resolver problemas.</span><span class="sxs-lookup"><span data-stu-id="a94d7-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="a94d7-105">Certifique-se de que a conta que aceitou o convite por e-mail é a mesma que está a ser usada para iniciar scontabilidade mais tarde.</span><span class="sxs-lookup"><span data-stu-id="a94d7-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="a94d7-106">Certifique-se de que o utilizador está a usar a mesma conta para aceitar o convite e assinar no site.</span><span class="sxs-lookup"><span data-stu-id="a94d7-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="a94d7-107">Para obter mais informações, consulte [Como gerir os pseudónimos da sua conta Microsoft </a> para gerir o login da Microsoft 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="a94d7-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Microsoft 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="a94d7-108">Navegue por cada site(s) em que o utilizador esteja a receber o erro.</span><span class="sxs-lookup"><span data-stu-id="a94d7-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="a94d7-109">Adicione "/_layouts/15/people.aspx/membershipgroupid=0" (dentro das cotações duplas) até ao final do URL do site.</span><span class="sxs-lookup"><span data-stu-id="a94d7-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="a94d7-110">Exemplo: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="a94d7-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="a94d7-111">Selecione o utilizador da lista.</span><span class="sxs-lookup"><span data-stu-id="a94d7-111">Select the user from the list.</span></span>

- <span data-ttu-id="a94d7-112">Clique **em Remover Permissões** do Utilizador da Fita.</span><span class="sxs-lookup"><span data-stu-id="a94d7-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="a94d7-113">Adicione de volta o Utilizador e reenvimente o convite ao utilizador.</span><span class="sxs-lookup"><span data-stu-id="a94d7-113">Add back the User and Resend the invite to the user.</span></span>

