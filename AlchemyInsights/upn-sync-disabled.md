---
title: UPN sincronizado
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 31947d7c491e4116ffdb9baadf286cd4fbb50f2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749525"
---
# <a name="upn-sync-disabled"></a>UPN sincronizado

Se começou a sincronizar a Azure AD antes de 30 de março de 2016, execute o seguinte cmdlet Azure AD PowerShell para ativar o soft match da UPN apenas para a sua organização:
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**
  
UPN soft match é automaticamente ligado para organizações que começaram a sincronizar a Azure AD em ou depois de 30 de março de 2016.
  
Para saber mais sobre como permitir uma partida suave na UPN e outras funcionalidades de sincronização, consulte [as funcionalidades do serviço de sincronização Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

