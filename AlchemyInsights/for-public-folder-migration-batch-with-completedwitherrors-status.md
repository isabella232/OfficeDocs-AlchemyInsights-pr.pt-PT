---
title: Para o lote de migração de pastas públicas com o estado CompletedWithErrors
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
ms.openlocfilehash: 78ceac80626159e72af5f9ac963365c5c057a4ef0de2b3dc7e4cde5e5cc155e5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54068175"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Para o lote de migração de pastas públicas com o estado CompletedWithErrors

Utilize os seguintes passos para concluir o lote, sem os itens grandes/incorreto: 
1. Aprovar os itens ignorados no lote de migração:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Utilize o seguinte comando para aprovar os itens ignorados em pedidos de migração que estão "Sincronizados" mas não concluídos:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. O lote de migração e os pedidos devem ser retomados e concluídos dentro de alguns minutos.

