---
title: Resolução de problemas Acesso negado mensagens ao OneDrive para sites empresariais
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9001cf0b7d9f1f05a2ecedca2c3137dd1b8a1c38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670627"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="fabaa-102">Resolução de problemas Acesso negado mensagens ao OneDrive para sites empresariais</span><span class="sxs-lookup"><span data-stu-id="fabaa-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="fabaa-103">Este problema ocorre mais frequentemente quando um utilizador é eliminado e recriado com o mesmo nome principal do utilizador (UPN).</span><span class="sxs-lookup"><span data-stu-id="fabaa-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="fabaa-104">A nova conta é criada utilizando um valor puid diferente (Passport Unique ID).</span><span class="sxs-lookup"><span data-stu-id="fabaa-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="fabaa-105">Quando o utilizador tenta aceder a uma coleção de sites ou ao seu OneDrive, o utilizador tem um PUID incorreto.</span><span class="sxs-lookup"><span data-stu-id="fabaa-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="fabaa-106">Um segundo cenário envolve a sincronização do diretório com uma unidade organizacional ative directy (OU).</span><span class="sxs-lookup"><span data-stu-id="fabaa-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="fabaa-107">Se os utilizadores já se inscreveram no SharePoint, e depois forem transferidos para um OU diferente e resincamados com o SharePoint, poderão experimentar este problema.</span><span class="sxs-lookup"><span data-stu-id="fabaa-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="fabaa-108">Para resolver este problema, deverá restaurar a UPN original com os passos do artigo, [Restaurar um utilizador na Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="fabaa-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>
2. <span data-ttu-id="fabaa-109">Se não conseguir restaurar o utilizador original, deve remover o utilizador antigo do site OneDrive utilizando estes passos, [Remova um utilizador da lista de informações do utilizador]().</span><span class="sxs-lookup"><span data-stu-id="fabaa-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="fabaa-110">Depois de feito, pode verificar se o utilizador tem direitos de administração para o site OneDrive, seguindo os passos para adicionar os [de administrador para o OneDrive de um utilizador](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span><span class="sxs-lookup"><span data-stu-id="fabaa-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span></span>

<span data-ttu-id="fabaa-111">Para obter mais informações sobre os níveis de permissão, consulte o artigo, [compreender os níveis de permissão no SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="fabaa-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
