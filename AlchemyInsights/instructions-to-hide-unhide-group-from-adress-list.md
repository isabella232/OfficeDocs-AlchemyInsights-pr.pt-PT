---
title: Instruções para ocultar/desagrupar grupo da lista de endereços
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: 02368d6a06df90d76ee1bd5448819e7ffe12c18c
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580020"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Esconda o grupo Microsoft 365 da lista de endereços (GAL)

Para ocultar um grupo Microsoft 365 das listas de endereços (GAL) de clientes exchange (como Outlook ou OWA), utilize o seguinte comando na concha EXO:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Para ocultar o grupo Microsoft 365 de ser visível para clientes Exchange, utilize o seguinte comando na concha EXO:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

