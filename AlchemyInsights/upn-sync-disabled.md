---
title: Sincronização de UPN desativada
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
ms.openlocfilehash: fc163fae4d348d7c7cf117bd457f999b42f96bec7c1eb9aa1435e346131d06de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038123"
---
# <a name="upn-sync-disabled"></a>Sincronização de UPN desativada

Se tiver começado a ser a mesma e o Azure AD antes de 30 de março de 2016, execute o seguinte cmdlet do PowerShell do Azure AD para ativar apenas a correspondência suave de UPN para a sua organização:
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**
  
A correspondência de atualizações upn é aativada automaticamente para as organizações que iniciaram a ascrianação com o Azure AD a partir de 30 de março de 2016.
  
Para saber mais sobre como ativar a funcionalidade de sincronização de upn e outras funcionalidades de sincronização, consulte O Azure AD Ligação funcionalidades do serviço [de sincronização.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)
  

