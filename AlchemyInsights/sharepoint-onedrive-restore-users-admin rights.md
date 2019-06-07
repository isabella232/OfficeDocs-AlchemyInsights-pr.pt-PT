---
title: Conceder acesso de utilizadores para SharePoint e OneDrive
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: a689769dab24e12832ddc0937bc5ddc3d71dbee3
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/07/2019
ms.locfileid: "34759266"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a><span data-ttu-id="6f1aa-102">Conceder acesso de utilizadores para SharePoint e OneDrive</span><span class="sxs-lookup"><span data-stu-id="6f1aa-102">Give users access to SharePoint and OneDrive</span></span>

<span data-ttu-id="6f1aa-103">Este problema ocorre com maior frequência quando um utilizador é eliminado e recriado com o mesmo nome principal de utilizador (UPN).</span><span class="sxs-lookup"><span data-stu-id="6f1aa-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="6f1aa-104">A nova conta é criada utilizando um valor diferente de PUID (ID exclusivo do Passport).</span><span class="sxs-lookup"><span data-stu-id="6f1aa-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="6f1aa-105">Quando o utilizador tenta aceder a uma colecção de sites ou seu OneDrive, o utilizador tem um PUID incorrecto.</span><span class="sxs-lookup"><span data-stu-id="6f1aa-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="6f1aa-106">Um segundo cenário envolve a sincronização de directório com uma unidade organizacional (UO) de Active Directory.</span><span class="sxs-lookup"><span data-stu-id="6f1aa-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="6f1aa-107">Se os utilizadores já iniciado sessão no SharePoint e, em seguida, são movidos para uma UO diferente e resynced com o SharePoint, eles poderão detectar este problema.</span><span class="sxs-lookup"><span data-stu-id="6f1aa-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="6f1aa-108">Para resolver este problema deve restaurar o UPN original com os passos no artigo[restaurar um utilizador no Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="6f1aa-108">To resolve this issue you should restore the original UPN with the steps in the article,[Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="6f1aa-109">Depois de fazer isto, pode verificar que o utilizador tem direitos de administrador para o site de OneDrive, seguindo os passos para [Adicionar administração para OneDrive um utilizador](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span><span class="sxs-lookup"><span data-stu-id="6f1aa-109">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span></span>

<span data-ttu-id="6f1aa-110">Para mais informações sobre níveis de permissão, consulte o artigo, [níveis de permissão de compreensão no SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="6f1aa-110">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
