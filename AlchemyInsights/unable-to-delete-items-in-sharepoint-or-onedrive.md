---
title: Não é possível eliminar itens no SharePoint ou OneDrive
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: 3cc168846999c6880b95edfaedb2df8cf6e843a6
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/04/2019
ms.locfileid: "36748586"
---
# <a name="unable-to-delete-items"></a>Não é possível eliminar itens

Problemas de eliminar itens do SharePoint?

- Sempre certificar-se de que tem as [permissões adequadas](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) para eliminar o item ou ter uma tentativa de [administrador da colecção de site](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) a remover o item.

- Certifique-se de que não existe uma definição de [política de retenção](https://docs.microsoft.com/office365/securitycompliance/retention-policies) no item.

- Certifique-se de que o item não está [reservado](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) para outro utilizador.

- Por último, os administradores podem utilizar o [SharePoint padrões e práticas](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) que contém uma biblioteca de comandos que lhe permitem executar acções de gestão complexos tais como forçar a eliminação de itens de stubborn do PowerShell.
- [Remover ficheiro PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Remover pasta PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Remover Item da lista de PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Remover lista de PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Remover PNP campo (coluna)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)