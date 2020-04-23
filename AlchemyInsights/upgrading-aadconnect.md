---
title: 932 Upgrade AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: fcc5fddb5cfd15407d0533449035317d187931ed
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766504"
---
# <a name="upgrade-azure-ad-connect"></a>Upgrade Azure AD Connect

Por predefinição, a atualização automática está ativada para o Azure AD Connect, o que ajuda a garantir que está a executar a versão mais recente. Para verificar as definições de atualização automática, utilize o **cmdlet Get-ADSyncAutoUpgrade** em Azure AD PowerShell. O cmdlet devolverá um dos seguintes valores:

- **Ativado**: Está ativada a atualização automática.

- **Desativado**: A atualização automática está desativada.

- **Suspenso**: O sistema já não é elegível para receber atualizações automáticas. Não é possível configurar este valor; é definido pelo sistema.

Para mais informações, consulte [a atualização automática](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Para descarregar a versão mais recente do [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594)Azure AD Connect, vá a .
