---
title: Remoção de problemas de mensagens negadas ao Access a OneDrive para Empresas sites
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
ms.openlocfilehash: fc4a2bd7dcc74f5f05e8b709e4bc3eac6ed445d6e2ea9ede698abbc8667723ce
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957804"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Remoção de problemas de mensagens negadas ao Access a OneDrive para Empresas sites

Este problema ocorre com mais frequência quando um utilizador é eliminado e recriado com o mesmo nome principal de utilizador (UPN). A nova conta é criada utilizando um valor PUID (Passaporte Exclusivo ID) diferente. Quando o utilizador tenta aceder a uma coleção de site ou à sua OneDrive, o utilizador tem um PUID incorreto. Um segundo cenário envolve a sincronização de diretórios com uma unidade organizacional do Active Directory (OU). Se os utilizadores já têm a sua primeira ação e, em seguida, foram movidos para um OU diferente e voltarem a silhá-lo com o SharePoint, poderão detetá-lo.

1. Para resolver este problema, deve restaurar o UPN original com os passos no artigo [Restaurar um utilizador no Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).
2. Se não conseguir restaurar o utilizador original, deve remover o utilizador antigo do site OneDrive através destes passos, Remover um utilizador da lista de [informações de utilizador](). 
3. Quando terminar, pode verificar se o utilizador tem direitos de administrador no site da OneDrive ao seguir os passos para Adicionar administradores para a conta de [um utilizador OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)

Para obter mais informações sobre níveis de permissão, consulte o artigo Compreender [os níveis de permissão no SharePoint.](https://docs.microsoft.com/sharepoint/understanding-permission-levels)
