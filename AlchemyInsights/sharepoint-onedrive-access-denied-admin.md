---
title: Solucionações de acesso negado mensagens
ms.author: pebaum
author: pebaum
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 57919e6dbd81a5bf3b17fb067485e8eec23b7d4c
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051436"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Soluciona-se o acesso negado mensagens no Sharepoint / OneDrive Admin Center

Se você estiver recebendo uma mensagem negada de acesso ao tentar navegar para um Sharepoint / OneDrive Admin Center, certifique-se de que você [atribuir uma licença para o usuário](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One). Se o usuário tiver uma licença, você também deve garantir que eles tenham [uma função](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) de administrador que possa acessar os centros de administração.

Esse problema também pode ocorrer quando um usuário é excluído e recriado com o mesmo nome principal do usuário (UPN). A nova conta é criada usando um valor puid diferente (Passport Unique ID). Quando o usuário tenta acessar uma coleção do site ou seu OneDrive, o usuário tem um PUID incorreto. Um segundo cenário envolve sincronização do diretório com uma unidade organizacional do Diretório Ativo (OU). Se os usuários já entraram no SharePoint e, em seguida, forem transferidos para uma OU diferente e resincronizados com o SharePoint, eles podem experimentar esse problema.

Para resolver esse problema, você deve restaurar a UPN original com as etapas do artigo, [restaurar um usuário no Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

Nota: Se um centro de administração OneDrive ou SharePoint não estiver disponível para vários usuários que tiveram acesso anteriormente, pode haver um problema de serviço temporário.  [Verifique o painel de saúde do serviço](https://portal.office.com/adminportal/home#/servicehealth).


