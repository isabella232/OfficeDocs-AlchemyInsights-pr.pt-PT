---
title: Instruções para esconder/desesconder o grupo da lista de endereços
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
ms.openlocfilehash: d0e0285701f1a5f308bdc682abaddf5cc2d34120
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768942"
---
# <a name="hide-office-365-group-from-address-list-gal"></a>Hide Office 365 grupo da lista de endereços (GAL)

Para ocultar um grupo do Office 365 das listas de endereços (GAL) dos clientes da Exchange (como outlook ou OWA), use o seguinte comando no escudo EXO:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Para esconder o grupo do Office 365 de ser visível para os clientes da Exchange, use o seguinte comando no escudo EXO:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

