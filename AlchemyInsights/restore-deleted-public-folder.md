---
title: Restaurar uma pasta pública eliminada
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3488"
ms.openlocfilehash: 6df196fc0bde37c962e3aa84dd602ee414dad3d329addfd16cb6e3dcc40fc2ae
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53943386"
---
# <a name="restore-a-deleted-public-folder"></a>Restaurar uma pasta pública eliminada

**Para restaurar itens eliminados a partir de uma pasta pública:**

- Consulte [Não é possível recuperar itens eliminados de uma pasta pública](https://aka.ms/pfrec)que não é de correio no Outlook 2016 .
 
**Para restaurar uma pasta pública eliminada (de qualquer tipo)**: 

- Utilize o seguinte comando do PowerShell do EXO:

    Sintaxe:

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Exemplo: O seguinte comando irá restaurar Subpata1 e colocar a mesma em \Parent1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Consulte [Restaurar uma pasta pública eliminada para](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) obter mais detalhes.
