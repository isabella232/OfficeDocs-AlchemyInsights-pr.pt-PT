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
# <a name="give-users-access-to-sharepoint-and-onedrive"></a>Conceder acesso de utilizadores para SharePoint e OneDrive

Este problema ocorre com maior frequência quando um utilizador é eliminado e recriado com o mesmo nome principal de utilizador (UPN). A nova conta é criada utilizando um valor diferente de PUID (ID exclusivo do Passport). Quando o utilizador tenta aceder a uma colecção de sites ou seu OneDrive, o utilizador tem um PUID incorrecto. Um segundo cenário envolve a sincronização de directório com uma unidade organizacional (UO) de Active Directory. Se os utilizadores já iniciado sessão no SharePoint e, em seguida, são movidos para uma UO diferente e resynced com o SharePoint, eles poderão detectar este problema.

Para resolver este problema deve restaurar o UPN original com os passos no artigo[restaurar um utilizador no Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

Depois de fazer isto, pode verificar que o utilizador tem direitos de administrador para o site de OneDrive, seguindo os passos para [Adicionar administração para OneDrive um utilizador](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)

Para mais informações sobre níveis de permissão, consulte o artigo, [níveis de permissão de compreensão no SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
