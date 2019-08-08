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
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Resolução de problemas de acesso negado mensagens para OneDrive para sites empresariais

Este problema ocorre com maior frequência quando um utilizador é eliminado e recriado com o mesmo nome principal de utilizador (UPN). A nova conta é criada utilizando um valor diferente de PUID (ID exclusivo do Passport). Quando o utilizador tenta aceder a uma colecção de sites ou seu OneDrive, o utilizador tem um PUID incorrecto. Um segundo cenário envolve a sincronização de directório com uma unidade organizacional (UO) de Active Directory. Se os utilizadores já iniciado sessão no SharePoint e, em seguida, são movidos para uma UO diferente e resynced com o SharePoint, eles poderão detectar este problema.

1. Para resolver este problema deve restaurar o UPN original com os passos no artigo[restaurar um utilizador no Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).
2. Se não conseguir restaurar o utilizador original deve remover o utilizador antigo do local do OneDrive com estes passos, [Remover um utilizador na lista de informações do utilizador](). 
3. Depois de fazer isto, pode verificar que o utilizador tem direitos de administrador para o site de OneDrive, seguindo os passos para [Adicionar administração para OneDrive um utilizador](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)

Para mais informações sobre níveis de permissão, consulte o artigo, [níveis de permissão de compreensão no SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
