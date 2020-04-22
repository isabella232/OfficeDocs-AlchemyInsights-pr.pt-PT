---
title: Problemas problemas - Utilizador não encontrado no diretório
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 3b863c5e9962dd29ca2ed41d113041d74830f615
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43702749"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="42e47-102">Problemas problemas - Utilizador não encontrado no diretório</span><span class="sxs-lookup"><span data-stu-id="42e47-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="42e47-103">Se os utilizadores estiverem a receber uma mensagem de erro "o utilizador não pode ser encontrado" no diretório, tente novamente onde o Tipo de Problema está o Utilizador não no diretório.</span><span class="sxs-lookup"><span data-stu-id="42e47-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="42e47-104">Os seguintes passos podem ser concluídos para resolver o problema.</span><span class="sxs-lookup"><span data-stu-id="42e47-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="42e47-105">Certifique-se de que a conta que aceitou o convite por e-mail é a mesma conta que está a ser usada para assinar mais tarde.</span><span class="sxs-lookup"><span data-stu-id="42e47-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="42e47-106">Certifique-se de que o utilizador está a usar a mesma conta para aceitar o convite e assinar no site.</span><span class="sxs-lookup"><span data-stu-id="42e47-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="42e47-107">Para mais informações, consulte como gerir pseudónimos para a [sua conta</a> Microsoft gerir o login Microsoft 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="42e47-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Microsoft 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="42e47-108">Navegue por cada site em que o utilizador esteja a receber o erro.</span><span class="sxs-lookup"><span data-stu-id="42e47-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="42e47-109">Adicione "/_layouts/15/people.aspx/membershipgroupid=0" (dentro das cotações duplas) ao final do URL do site.</span><span class="sxs-lookup"><span data-stu-id="42e47-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="42e47-110">Exemplo: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="42e47-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="42e47-111">Selecione o utilizador da lista.</span><span class="sxs-lookup"><span data-stu-id="42e47-111">Select the user from the list.</span></span>

- <span data-ttu-id="42e47-112">Clique em **remover permissões** de utilizador da fita.</span><span class="sxs-lookup"><span data-stu-id="42e47-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="42e47-113">Adicione de volta o Utilizador e reenvie o convite para o utilizador.</span><span class="sxs-lookup"><span data-stu-id="42e47-113">Add back the User and Resend the invite to the user.</span></span>

