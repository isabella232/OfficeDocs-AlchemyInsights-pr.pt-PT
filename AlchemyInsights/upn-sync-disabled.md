---
title: UPN sincronizado
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 2b1ba772459091ce1a796884997fe2516d0407eb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782162"
---
# <a name="upn-sync-disabled"></a>UPN sincronizado

Se começou a sincronizar a Azure AD antes de 30 de março de 2016, execute o seguinte cmdlet Azure AD PowerShell para ativar o soft match da UPN apenas para a sua organização:
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**
  
UPN soft match é automaticamente ligado para organizações que começaram a sincronizar a Azure AD em ou depois de 30 de março de 2016.
  
Para saber mais sobre como permitir uma partida suave na UPN e outras funcionalidades de sincronização, consulte [as funcionalidades do serviço de sincronização Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

