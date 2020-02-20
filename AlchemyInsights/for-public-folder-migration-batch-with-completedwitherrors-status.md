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
ms.openlocfilehash: 739e9d91f90e4c0374814d199e4372eb5625553a
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158628"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Para o lote de migração de pastas públicas com o estatuto CompletedWithErrors

Utilize os seguintes passos para completar o lote, saltando os itens grandes/maus: 
1. Aprove os itens ignorados no lote de migração:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Utilize o seguinte comando para aprovar os itens ignorados em pedidos de migração que são "Sincronizados" mas não concluídos:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. O lote de migração e os pedidos devem ser retomados e concluídos em poucos minutos.

