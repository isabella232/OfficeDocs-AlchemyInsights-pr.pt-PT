---
title: Para lote de migração de pastas públicas com estatuto de ConcluídoWithErrors
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
- "3532"
ms.openlocfilehash: 9ed21bfb9069b56a4fc59b201bb3ad94c6bb6712
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812475"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Para lote de migração de pastas públicas com estatuto de ConcluídoWithErrors

Utilize os seguintes passos para completar o lote, saltando os itens grandes/maus: 
1. Aprovar os itens ignorados no lote de migração:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Utilize o seguinte comando para aprovar os itens ignorados em pedidos de migração que são "Sincronizados" mas não concluídos:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. O lote de migração e os pedidos devem ser retomados e completos em poucos minutos.

