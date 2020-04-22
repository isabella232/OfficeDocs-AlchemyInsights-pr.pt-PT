---
title: Sincronizado UPN
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 33bc7e30d41ff70e2ce55d946202acf45dbcb0f2
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43726115"
---
# <a name="upn-sync-disabled"></a>Sincronizado UPN

Se começou a sincronizar com a Azure AD antes de 30 de março de 2016, execute o seguinte cmdlet Azure AD PowerShell para permitir a upn soft match apenas para a sua organização:
  
 **Set-MsolDirSyncFeature -Funcionalidade ActivadorsoftMatchOnUpn -Enable $True**
  
Upn soft match é automaticamente ativado para organizações que começaram a sincronizar com Azure AD em ou depois de 30 de março de 2016.
  
Para saber mais sobre permitir uma correspondência suave na UPN e outras funcionalidades de sincronização, consulte as funcionalidades de [sincronização do Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

