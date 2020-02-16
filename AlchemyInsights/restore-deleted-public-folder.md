---
title: Restaurar uma pasta pública eliminada
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3488"
ms.openlocfilehash: 7b04612daca61650d162c1dde240e25c1b185b04
ms.sourcegitcommit: 8ba12eff67e405f5922ea4cc35155e3036447859
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/15/2020
ms.locfileid: "42063718"
---
# <a name="restore-a-deleted-public-folder"></a>Restaurar uma pasta pública eliminada

**Para restaurar os itens apagados de uma pasta pública:**

- Ver [Não pode recuperar itens apagados de uma pasta pública não-mail no Outlook 2016](https://aka.ms/pfrec).
 
**Para restaurar uma pasta pública eliminada (de qualquer tipo)**: 

- Utilize o seguinte comando EXO PowerShell:

    Sintaxe:

    >$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse [ ? {$_. Nome -eq\<" name_of_deleted_public_Folder"}; Set-PublicFolder $pf.identity \<-Path path where the folder will be restored>

    Exemplo: O seguinte comando restaurará a Subpasta1 e colocá-la-á em \Parent1:

    >$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse [ ? {$_. Nome -eq "Subpasta1"}; Set-PublicFolder $pf.identity -Path \Parent1

Consulte [restaurar uma pasta pública eliminada](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) para obter mais detalhes.
