---
title: Resolução de problemas Acesso negado mensagens ao OneDrive para sites empresariais
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 95bd46e8b7a6006f3735612d9a5602fb2b2a283b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511195"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Resolução de problemas Acesso negado mensagens ao OneDrive para sites empresariais

Este problema ocorre mais frequentemente quando um utilizador é eliminado e recriado com o mesmo nome principal do utilizador (UPN). A nova conta é criada utilizando um valor puid diferente (Passport Unique ID). Quando o utilizador tenta aceder a uma coleção de sites ou ao seu OneDrive, o utilizador tem um PUID incorreto. Um segundo cenário envolve a sincronização do diretório com uma unidade organizacional ative directy (OU). Se os utilizadores já se inscreveram no SharePoint, e depois forem transferidos para um OU diferente e resincamados com o SharePoint, poderão experimentar este problema.

1. Para resolver este problema, deverá restaurar a UPN original com os passos do artigo, [Restaurar um utilizador na Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).
2. Se não conseguir restaurar o utilizador original, deve remover o utilizador antigo do site OneDrive utilizando estes passos, [Remova um utilizador da lista de informações do utilizador](). 
3. Depois de feito, pode verificar se o utilizador tem direitos de administração para o site OneDrive, seguindo os passos para adicionar os [de administrador para o OneDrive de um utilizador](https://docs.microsoft.com/sharepoint/manage-user-profiles)

Para obter mais informações sobre os níveis de permissão, consulte o artigo, [compreender os níveis de permissão no SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
