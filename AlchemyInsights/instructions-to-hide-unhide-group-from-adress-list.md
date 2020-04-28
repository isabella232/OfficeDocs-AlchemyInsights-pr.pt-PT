---
title: Instruções para ocultar/desocultar grupo da lista de endereços
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
ms.openlocfilehash: 61ba34e6d554831da712a92401f26fabb02c26b7
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/27/2020
ms.locfileid: "43908355"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Ocultar o grupo Microsoft 365 da lista de endereços (GAL)

Para ocultar um grupo Microsoft 365 das listas de endereços (GAL) dos clientes Exchange (como outlook ou OWA), utilize o seguinte comando na concha EXO:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Para esconder que o grupo Microsoft 365 seja visível para os clientes Exchange, utilize o seguinte comando na concha EXO:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

