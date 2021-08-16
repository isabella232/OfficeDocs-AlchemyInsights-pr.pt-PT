---
title: Não é possível eliminar itens no SharePoint ou no OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: 3601c5eff121e10b6bddace6f7228204a01080a636e24f3a56373fe8d469c799
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038528"
---
# <a name="unable-to-delete-items"></a>Não é possível eliminar itens

- As políticas de retenção podem causar este problema, pelo que tem de desativar ou excluir as respetivas respetivas retenção que estão a causar este problema. Após a remoção de uma política de retenção ou de uma retenção, poderá demorar até 24 horas para que a alteração entre em vigor. Certifique-se de que não [existe uma configuração de](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) política de retenção no item.

- O site pode ter excedido o limite de armazenamento, aumentar [a quota do site](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) e eliminar o item.

- Certifique-se de que o item [não tem saída para](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) outro utilizador.

- Por fim, os administradores podem utilizar os Padrões e Práticas do [SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP), que contém uma biblioteca de comandos do PowerShell que lhe permitem efetuar ações de gestão complexas, como forçar a eliminação de itens de preparação.
- [Remover Ficheiro PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Remover Pasta PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Remover Item de Lista PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Remover Lista PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Remover Campo PNP (Coluna)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)