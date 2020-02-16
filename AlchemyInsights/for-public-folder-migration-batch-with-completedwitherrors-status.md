---
title: Para o lote de migração de pastas públicas com o estatuto CompletedWithErrors
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
- "3532"
ms.openlocfilehash: 4243cdf0170fed1eadac6560d2a04e1a861c63e5
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/15/2020
ms.locfileid: "42043609"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Para o lote de migração de pastas públicas com o estatuto CompletedWithErrors

Utilize os seguintes passos para completar o lote, saltando os itens grandes/maus: 
1. Aprove os itens ignorados no lote de migração:

    Set-MigrationBatch \<nome de lote> -ApproveSkippedItems 
2. Utilize o seguinte comando para aprovar os itens ignorados em pedidos de migração que são "Sincronizados" mas não concluídos:

    $pf=Get-PublicFolderMailboxMigrationRequest [ Get-PublicFolderMailboxMigrationRequest] Get-PublicFolderMailboxMigrationRequestStatistics -IncluirRelatório; ForEach ($i em $pf) {se ($i.LargeItemsEncountered -gt 0 -ou $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([[DataTime]:UtcNow)}}
3. O lote de migração e os pedidos devem ser retomados e concluídos em poucos minutos.

