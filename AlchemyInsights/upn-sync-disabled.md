---
title: Sincronização UPN desactivada
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: d00f10688ec775c22d60a9089e291c265ada46f1
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/15/2019
ms.locfileid: "28306353"
---
# <a name="upn-sync-disabled"></a>Sincronização UPN desactivada

Se iniciar a sincronização com AD Azure antes de 30 de Março de 2016, execute o cmdlet Azure AD PowerShell seguinte para activar a correspondência de software de UPN para a sua organização apenas:
  
 **Conjunto-MsolDirSyncFeature-funcionalidade EnableSoftMatchOnUpn-activar $True**
  
Correspondência de software de UPN é automaticamente activada para organizações que iniciou a sincronização com AD Azure em ou após 30 de Março de 2016.
  
Para obter mais informações sobre como activar a correspondência com software UPN e outras funcionalidades de sincronização, consulte [funcionalidades de suporte de sincronização Azure AD ligar](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

