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
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Resolução de problemas Acesso negado mensagens ao OneDrive para sites empresariais

Este problema ocorre mais frequentemente quando um utilizador é eliminado e recriado com o mesmo nome principal do utilizador (UPN). A nova conta é criada utilizando um valor puid diferente (Passport Unique ID). Quando o utilizador tenta aceder a uma coleção de sites ou ao seu OneDrive, o utilizador tem um PUID incorreto. Um segundo cenário envolve a sincronização do diretório com uma unidade organizacional ative directy (OU). Se os utilizadores já se inscreveram no SharePoint, e depois forem transferidos para um OU diferente e resincamados com o SharePoint, poderão experimentar este problema.

1. Para resolver este problema, deverá restaurar a UPN original com os passos do artigo, [Restaurar um utilizador na Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).
2. Se não conseguir restaurar o utilizador original, deve remover o utilizador antigo do site OneDrive utilizando estes passos, [Remova um utilizador da lista de informações do utilizador](). 
3. Depois de feito, pode verificar se o utilizador tem direitos de administração para o site OneDrive, seguindo os passos para adicionar os [de administrador para o OneDrive de um utilizador](https://docs.microsoft.com/sharepoint/manage-user-profiles)

Para obter mais informações sobre os níveis de permissão, consulte o artigo, [compreender os níveis de permissão no SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
