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
ms.openlocfilehash: db45aa8df40484fdcda7c430f1ca27482a1dd4ce
ms.sourcegitcommit: a9415f3ae8c7ba267b5134bcbdc1e070cea41a0f
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/12/2020
ms.locfileid: "49019594"
---
# <a name="unable-to-delete-items"></a>Incapaz de eliminar itens

- As políticas de retenção podem causar isto, você precisa desativar ou excluir o respetivo hold que está causando este problema. Depois de uma política de retenção ou detenção ser removida, pode levar até 24 horas para que a alteração entre em vigor. Certifique-se de que não existe uma configuração da política de [retenção](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) no item.

- O site pode ter excedido o limite de armazenamento, aumentar a quota do [site](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) e apagar o item.

- Certifique-se de que o artigo não é [verificado](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) a outro utilizador.

- Finalmente, os administradores podem usar [Padrões e Práticas sharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) que contém uma biblioteca de comandos PowerShell que lhe permitem executar ações de gestão complexas, tais como a eliminação de itens teimosos.
- [Remover Arquivo PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Remover pasta PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Remover item da lista PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Remover lista PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Remover campo PNP (Coluna)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)