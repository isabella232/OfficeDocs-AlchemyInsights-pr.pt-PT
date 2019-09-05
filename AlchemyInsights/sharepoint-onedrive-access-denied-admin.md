---
title: Resolver mensagens de acesso negado
ms.author: pebaum
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 4e6fdc6fbf745d1702bf1a7b3474ac82f6662305
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/04/2019
ms.locfileid: "36751287"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Resolução de problemas de acesso negado mensagens no Centro de administração do Sharepoint/OneDrive

Se estiver a receber uma mensagem de acesso negado ao tentar navegar para um centro de administração do Sharepoint/OneDrive, certifique-se que [atribua uma licença para o utilizador](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One). Se o utilizador tiver uma licença, deve também certificar-se de que são [atribuídos uma função de administrador](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) que pode aceder os centros de admin.

Este problema também pode ocorrer quando um utilizador é eliminado e recriado com o mesmo nome principal de utilizador (UPN). A nova conta é criada utilizando um valor diferente de PUID (ID exclusivo do Passport). Quando o utilizador tenta aceder a uma colecção de sites ou seu OneDrive, o utilizador tem um PUID incorrecto. Um segundo cenário envolve a sincronização de directório com uma unidade organizacional (UO) de Active Directory. Se os utilizadores já iniciado sessão no SharePoint e, em seguida, são movidos para uma UO diferente e resynced com o SharePoint, eles poderão detectar este problema.

Para resolver este problema, deverá restaurar o UPN original com os passos no artigo [restaurar um utilizador no Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

Nota: Se um centro de OneDrive ou de administração do SharePoint não está disponível para vários utilizadores, que tinham anteriormente acesso, poderá existir um problema de serviço temporária.  [Verifique o dashboard de estado de funcionamento do serviço](https://portal.office.com/adminportal/home#/servicehealth).


