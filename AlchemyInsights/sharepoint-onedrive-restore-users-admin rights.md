---
title: Resolução de problemas de acesso negado mensagens para OneDrive para sites empresariais
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: d47ce80bdd07a25d9724057edf0289808a00a3db
ms.sourcegitcommit: 8a83b508785c96c19648ed574f442bbef2c2dff9
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/07/2019
ms.locfileid: "36232545"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="4d7bb-102">Resolução de problemas de acesso negado mensagens para OneDrive para sites empresariais</span><span class="sxs-lookup"><span data-stu-id="4d7bb-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="4d7bb-103">Este problema ocorre com maior frequência quando um utilizador é eliminado e recriado com o mesmo nome principal de utilizador (UPN).</span><span class="sxs-lookup"><span data-stu-id="4d7bb-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="4d7bb-104">A nova conta é criada utilizando um valor diferente de PUID (ID exclusivo do Passport).</span><span class="sxs-lookup"><span data-stu-id="4d7bb-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="4d7bb-105">Quando o utilizador tenta aceder a uma colecção de sites ou seu OneDrive, o utilizador tem um PUID incorrecto.</span><span class="sxs-lookup"><span data-stu-id="4d7bb-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="4d7bb-106">Um segundo cenário envolve a sincronização de directório com uma unidade organizacional (UO) de Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4d7bb-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="4d7bb-107">Se os utilizadores já iniciado sessão no SharePoint e, em seguida, são movidos para uma UO diferente e resynced com o SharePoint, eles poderão detectar este problema.</span><span class="sxs-lookup"><span data-stu-id="4d7bb-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="4d7bb-108">Para resolver este problema deve restaurar o UPN original com os passos no artigo[restaurar um utilizador no Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="4d7bb-108">To resolve this issue you should restore the original UPN with the steps in the article,[Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>
2. <span data-ttu-id="4d7bb-109">Se não conseguir restaurar o utilizador original deve remover o utilizador antigo do local do OneDrive com estes passos, [Remover um utilizador na lista de informações do utilizador]().</span><span class="sxs-lookup"><span data-stu-id="4d7bb-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="4d7bb-110">Depois de fazer isto, pode verificar que o utilizador tem direitos de administrador para o site de OneDrive, seguindo os passos para [Adicionar administração para OneDrive um utilizador](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span><span class="sxs-lookup"><span data-stu-id="4d7bb-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span></span>

<span data-ttu-id="4d7bb-111">Para mais informações sobre níveis de permissão, consulte o artigo, [níveis de permissão de compreensão no SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="4d7bb-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
