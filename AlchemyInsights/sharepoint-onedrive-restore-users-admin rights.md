---
title: Solução de problemas Acesso negado mensagens para OneDrive para sites de negócios
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9d8aba4e53a1e0505a430296bb1c11713ea2ce7b
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051616"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Solução de problemas Acesso negado mensagens para OneDrive para sites de negócios

Esse problema ocorre com mais frequência quando um usuário é excluído e recriado com o mesmo nome principal do usuário (UPN). A nova conta é criada usando um valor puid diferente (Passport Unique ID). Quando o usuário tenta acessar uma coleção do site ou seu OneDrive, o usuário tem um PUID incorreto. Um segundo cenário envolve sincronização do diretório com uma unidade organizacional do Diretório Ativo (OU). Se os usuários já entraram no SharePoint e, em seguida, forem transferidos para uma OU diferente e resincronizados com o SharePoint, eles podem experimentar esse problema.

1. Para resolver esse problema, você deve restaurar a UPN original com as etapas do artigo, [restaure um usuário no Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).
2. Se você não puder restaurar o usuário original, você deve remover o usuário antigo do site OneDrive usando essas etapas, [retire um usuário da lista de informações do usuário.]() 
3. Depois que isso for feito, você pode verificar se o usuário tem direitos de administração para o site OneDrive, seguindo as etapas para [adicionar admin's para onedrive de um usuário](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)

Para obter mais informações sobre os níveis de permissão, consulte o artigo, [entendendo os níveis de permissão no SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
