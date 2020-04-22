---
title: Acesso de problemas Mensagens negadas
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 82e11458529b8a49e583b1a6963a51e2a466bfd6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758493"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Acesso de problemas Mensagens negadas no Sharepoint/OneDrive Admin Center

Se estiver a receber uma mensagem negada de acesso ao tentar navegar para um Sharepoint/OneDrive Admin Center, certifique-se de que [atribui uma licença ao utilizador](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One). Se o utilizador tiver uma licença, deve também certificar-se de que lhes é [atribuída uma função](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) de administrador que possa aceder aos centros de administração.

Este problema também pode ocorrer quando um utilizador é eliminado e recriado com o mesmo nome principal do utilizador (UPN). A nova conta é criada utilizando um valor DIFERENTE de PUID (Id Exclusivo passaporte). Quando o utilizador tenta aceder a uma recolha do site ou ao seu OneDrive, o utilizador tem um PUID incorreto. Um segundo cenário envolve a sincronização do diretório com uma unidade organizacional do Diretório Ativo (OU). Se os utilizadores já se inscreveram no SharePoint, e depois são transferidos para um OU diferente e resincronizados com o SharePoint, podem experimentar este problema.

Para resolver este problema, deve restaurar a UPN original com os passos do artigo, [Restaurar um utilizador na Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

Nota: Se um centro de administração OneDrive ou SharePoint não estiver disponível para vários utilizadores que anteriormente tiveram acesso, pode haver um problema de serviço temporário.  [Verifique o painel de saúde do serviço.](https://portal.office.com/adminportal/home#/servicehealth)


