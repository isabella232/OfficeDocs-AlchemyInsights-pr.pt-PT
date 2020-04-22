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
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Resolução de problemas O Acesso negou mensagens ao OneDrive para sites de negócios

Este problema ocorre com mais frequência quando um utilizador é eliminado e recriado com o mesmo nome principal do utilizador (UPN). A nova conta é criada utilizando um valor DIFERENTE de PUID (Id Exclusivo passaporte). Quando o utilizador tenta aceder a uma recolha do site ou ao seu OneDrive, o utilizador tem um PUID incorreto. Um segundo cenário envolve a sincronização do diretório com uma unidade organizacional do Diretório Ativo (OU). Se os utilizadores já se inscreveram no SharePoint, e depois são transferidos para um OU diferente e resincronizados com o SharePoint, podem experimentar este problema.

1. Para resolver este problema, deve restaurar a UPN original com os passos do artigo, [Restaurar um utilizador na Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).
2. Se não conseguir restaurar o utilizador original, deve retirar o antigo utilizador do site OneDrive utilizando estas etapas, [Remova um utilizador da lista de informações do utilizador](). 
3. Depois de feito, pode verificar se o utilizador tem direitos de administração no site oneDrive seguindo os passos para [adicionar administradores para o OneDrive de um utilizador](https://docs.microsoft.com/sharepoint/manage-user-profiles)

Para obter mais informações sobre os níveis de permissão, consulte o artigo, Compreender os níveis de [permissão no SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
