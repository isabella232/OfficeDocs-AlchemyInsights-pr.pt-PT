---
title: Para lote de migração de pastas públicas com estatuto de ConcluídoWithErrors
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3532"
ms.openlocfilehash: cbf5237fdb5c660057465e67702e35f68e545ddb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744124"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a><span data-ttu-id="81095-102">Para lote de migração de pastas públicas com estatuto de ConcluídoWithErrors</span><span class="sxs-lookup"><span data-stu-id="81095-102">For Public folder migration batch with CompletedWithErrors status</span></span>

<span data-ttu-id="81095-103">Utilize os seguintes passos para completar o lote, saltando os itens grandes/maus:</span><span class="sxs-lookup"><span data-stu-id="81095-103">Use the following steps to complete the batch, skipping the large/bad items:</span></span> 
1. <span data-ttu-id="81095-104">Aprovar os itens ignorados no lote de migração:</span><span class="sxs-lookup"><span data-stu-id="81095-104">Approve the skipped items on migration batch:</span></span>

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. <span data-ttu-id="81095-105">Utilize o seguinte comando para aprovar os itens ignorados em pedidos de migração que são "Sincronizados" mas não concluídos:</span><span class="sxs-lookup"><span data-stu-id="81095-105">Use the following command to approve the skipped items on migration requests that are “Synced” but not completed:</span></span>

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. <span data-ttu-id="81095-106">O lote de migração e os pedidos devem ser retomados e completos em poucos minutos.</span><span class="sxs-lookup"><span data-stu-id="81095-106">The migration batch and requests should resume and complete in a few minutes.</span></span>

