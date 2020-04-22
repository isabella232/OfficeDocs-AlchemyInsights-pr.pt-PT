---
title: Resolução de problemas O Acesso negou mensagens ao OneDrive para sites de negócios
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: a83936acf969926c113b28ceb22b006cdb96e2b4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692812"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="e91a0-102">Resolução de problemas O Acesso negou mensagens ao OneDrive para sites de negócios</span><span class="sxs-lookup"><span data-stu-id="e91a0-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="e91a0-103">Este problema ocorre com mais frequência quando um utilizador é eliminado e recriado com o mesmo nome principal do utilizador (UPN).</span><span class="sxs-lookup"><span data-stu-id="e91a0-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="e91a0-104">A nova conta é criada utilizando um valor DIFERENTE de PUID (Id Exclusivo passaporte).</span><span class="sxs-lookup"><span data-stu-id="e91a0-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="e91a0-105">Quando o utilizador tenta aceder a uma recolha do site ou ao seu OneDrive, o utilizador tem um PUID incorreto.</span><span class="sxs-lookup"><span data-stu-id="e91a0-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="e91a0-106">Um segundo cenário envolve a sincronização do diretório com uma unidade organizacional do Diretório Ativo (OU).</span><span class="sxs-lookup"><span data-stu-id="e91a0-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="e91a0-107">Se os utilizadores já se inscreveram no SharePoint, e depois são transferidos para um OU diferente e resincronizados com o SharePoint, podem experimentar este problema.</span><span class="sxs-lookup"><span data-stu-id="e91a0-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="e91a0-108">Para resolver este problema, deve restaurar a UPN original com os passos do artigo, [Restaurar um utilizador na Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="e91a0-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>
2. <span data-ttu-id="e91a0-109">Se não conseguir restaurar o utilizador original, deve retirar o antigo utilizador do site OneDrive utilizando estas etapas, [Remova um utilizador da lista de informações do utilizador]().</span><span class="sxs-lookup"><span data-stu-id="e91a0-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="e91a0-110">Depois de feito, pode verificar se o utilizador tem direitos de administração no site oneDrive seguindo os passos para [adicionar administradores para o OneDrive de um utilizador](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span><span class="sxs-lookup"><span data-stu-id="e91a0-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span></span>

<span data-ttu-id="e91a0-111">Para obter mais informações sobre os níveis de permissão, consulte o artigo, Compreender os níveis de [permissão no SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="e91a0-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
