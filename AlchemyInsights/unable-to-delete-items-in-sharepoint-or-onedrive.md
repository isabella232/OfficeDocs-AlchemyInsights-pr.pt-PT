---
title: Não é possível excluir itens no SharePoint ou no OneDrive
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
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/18/2019
ms.locfileid: "36748586"
---
# <a name="unable-to-delete-items"></a>Não é possível excluir itens

Tendo problemas ao excluir itens do SharePoint?

- Certifique-se sempre de que tem as [permissões apropriadas](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) para eliminar o item ou ter uma tentativa de [administrador de conjunto de sites](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) remover o item.

- Certifique-se de que não exista uma configuração [de política de retenção](https://docs.microsoft.com/office365/securitycompliance/retention-policies) no item.

- Verifique se o item não está com [check-out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) para outro usuário.

- Finalmente, os administradores podem usar [padrões e práticas do SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) que contém uma biblioteca de comandos do PowerShell que permitem executar ações de gerenciamento complexas, como forçar a exclusão de itens persistentes.
- [Remover arquivo PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Remover pasta PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Remover item de lista PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Remover lista PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Remover campo PNP (coluna)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)