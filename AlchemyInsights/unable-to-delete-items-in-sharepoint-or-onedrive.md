---
title: Incapaz de eliminar itens no SharePoint ou OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: abfcb91c6040aeed759d697ca63546ccea8ede97
ms.sourcegitcommit: c5e800313a6f211386a384716e5fa18e7fcc8c1c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/28/2020
ms.locfileid: "41571282"
---
# <a name="unable-to-delete-items"></a>Incapaz de apagar itens

As políticas de retenção podem causar isso, você precisa de desativar ou excluir o respetivo porão que está a causar este problema. Após a remoção de uma política de retenção ou de espera, pode demorar até 24 horas para que a alteração entre em vigor. Certifique-se de que não existe uma definição de política de [retenção](https://docs.microsoft.com/office365/securitycompliance/retention-policies) no artigo.

O site pode ter excedido o limite de armazenamento, aumentado a quota do [site](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) e apagado o item.

Certifique-se de que o artigo não é [verificado](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) a outro utilizador.

Finalmente, os administradores podem usar [Padrões e Práticas SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) que contém uma biblioteca de comandos PowerShell que lhe permitem realizar ações de gestão complexas, tais como a eliminação de itens teimosos.
- [Remover ficheiro PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Remover pasta PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Remover o item da lista PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Remover a lista pnp](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Remover o campo PNP (Coluna)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)