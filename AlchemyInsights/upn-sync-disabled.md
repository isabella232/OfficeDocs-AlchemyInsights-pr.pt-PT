---
title: Sincronização UPN desactivada
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 983796ce8fb7e8b52c0ce31aa13597b53cc9e038
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/12/2019
ms.locfileid: "29921719"
---
# <a name="upn-sync-disabled"></a>Sincronização UPN desactivada

Se iniciar a sincronização com AD Azure antes de 30 de Março de 2016, execute o cmdlet Azure AD PowerShell seguinte para activar a correspondência de software de UPN para a sua organização apenas:
  
 **Conjunto-MsolDirSyncFeature-funcionalidade EnableSoftMatchOnUpn-activar $True**
  
Correspondência de software de UPN é automaticamente activada para organizações que iniciou a sincronização com AD Azure em ou após 30 de Março de 2016.
  
Para obter mais informações sobre como activar a correspondência com software UPN e outras funcionalidades de sincronização, consulte [funcionalidades de suporte de sincronização Azure AD ligar](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

