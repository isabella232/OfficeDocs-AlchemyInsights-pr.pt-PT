---
title: Ocultar ou mostrar os grupos do Office 365 ou equipas da lista de endereços
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002947"
- "5642"
ms.openlocfilehash: 7e667e22cd81f38a1a2c1385bf42e5227cb641480f4b505110ee7349a13f13a1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088407"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a>Ocultar ou mostrar os grupos do Office 365 ou equipas da lista de endereços

Utilize o seguinte comando EXO do Windows PowerShell para ocultar ou mostrar o grupo/equipas do Office 365 das listas de endereços (GAL) dos clientes do Exchange (Outlook, OWA):

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

Utilize o seguinte comando EXO do Windows PowerShell para ocultar ou mostrar o grupo/equipas do Office 365 dos clientes do Exchange (Outlook, OWA):

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- Para obter instruções detalhadas, consulte [Ocultar Grupos do Office 365 da GAL e dos clientes do Exchange](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal).
