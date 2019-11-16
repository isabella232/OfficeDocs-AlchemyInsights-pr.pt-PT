---
title: Problema de solucionamento de problemas - Usuário não encontrado no diretório
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 59713231da25be441e7c05d788337e66bf17265a
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/15/2019
ms.locfileid: "37768812"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="23ebd-102">Problema de solucionamento de problemas - Usuário não encontrado no diretório</span><span class="sxs-lookup"><span data-stu-id="23ebd-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="23ebd-103">Se os usuários estiverem recebendo mensagem de erro "o usuário não pode ser encontrado" no diretório, tente novamente onde o tipo de edição não está no diretório.</span><span class="sxs-lookup"><span data-stu-id="23ebd-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="23ebd-104">As seguintes etapas podem ser concluídas para solucionar o problema.</span><span class="sxs-lookup"><span data-stu-id="23ebd-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="23ebd-105">Certifique-se de que a conta que aceitou o convite por e-mail é a mesma conta que está sendo usada para entrar mais tarde.</span><span class="sxs-lookup"><span data-stu-id="23ebd-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="23ebd-106">Certifique-se de que o usuário está usando a mesma conta para aceitar o convite e entrar no site.</span><span class="sxs-lookup"><span data-stu-id="23ebd-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="23ebd-107">Para mais informações, veja [como gerenciar pseudônimos para sua conta</a> da Microsoft para gerenciar o login do Office 365.](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases)</span><span class="sxs-lookup"><span data-stu-id="23ebd-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="23ebd-108">Navegue para cada site (s) em que o usuário está recebendo o erro.</span><span class="sxs-lookup"><span data-stu-id="23ebd-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="23ebd-109">Adicione "/_layouts/15/people.aspx/membershipgroupid=0" (dentro das cotações duplas) até o final da URL do site.</span><span class="sxs-lookup"><span data-stu-id="23ebd-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="23ebd-110">Exemplo: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="23ebd-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="23ebd-111">Selecione o usuário da lista.</span><span class="sxs-lookup"><span data-stu-id="23ebd-111">Select the user from the list.</span></span>

- <span data-ttu-id="23ebd-112">Clique **em remover as permissões** do usuário da fita.</span><span class="sxs-lookup"><span data-stu-id="23ebd-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="23ebd-113">Adicione de volta o usuário e reenviar o convite para o usuário.</span><span class="sxs-lookup"><span data-stu-id="23ebd-113">Add back the User and Resend the invite to the user.</span></span>

