---
title: Instruções para ocultar/desagrupar grupo da lista de endereços
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
- "1200024"
- "3161"
ms.openlocfilehash: 4d55866700b9b8494f1f692cd3b865116b96a1bc
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831889"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Esconda o grupo Microsoft 365 da lista de endereços (GAL)

Para ocultar um grupo Microsoft 365 das listas de endereços (GAL) de clientes exchange (como Outlook ou OWA), utilize o seguinte comando na concha EXO:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Para ocultar o grupo Microsoft 365 de ser visível para clientes Exchange, utilize o seguinte comando na concha EXO:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

