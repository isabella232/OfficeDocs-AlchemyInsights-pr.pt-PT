---
title: 932 AADConnect actualizar
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 932
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 210f230929db72027a0f729b17901fe88eb45709
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/07/2019
ms.locfileid: "34757302"
---
# <a name="upgrade-azure-ad-connect"></a>Actualização Azure AD ligar

Por predefinição, a actualização automática está activada para Azure ligar AD, que ajuda a garantir está a executar a versão mais recente. Para verificar as definições de actualização automáticas, utilize o cmdlet **Get-ADSyncAutoUpgrade** no PowerShell de AD Azure. O cmdlet irá devolver um dos seguintes valores: 

- **Activado**: actualização automática está activada.

- **Desactivado**: actualização automática está desactivada.

- **Suspenso**: O sistema já não é elegível para receber actualizações automáticas. Não é possível configurar este valor; é definida pelo sistema. 

Para mais informações, consulte [actualização automática](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Para transferir a versão mais recente do Azure AD ligar, vá para [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).
