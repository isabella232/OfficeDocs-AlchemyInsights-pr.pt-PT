---
title: 932 Upgrade AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 5c8ec5d9282c53c655e28f5d38fe36fc3ab005b8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806050"
---
# <a name="upgrade-azure-ad-connect"></a>Upgrade Azure AD Connect

Por predefinição, a atualização automática está ativada para o Azure AD Connect, o que ajuda a garantir que está a executar a versão mais recente. Para verificar as definições de atualização automática, utilize o cmdlet **Get-ADSyncAutoUpgrade** em Azure AD PowerShell. O cmdlet devolverá um dos seguintes valores:

- **Ativado**: A atualização automática está ativada.

- **Desativado:** A atualização automática está desativada.

- **Suspenso**: O sistema já não é elegível para receber atualizações automáticas. Não pode configurar este valor; é definido pelo sistema.

Para mais informações, consulte [a atualização automática.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)

Para descarregar a versão mais recente do Azure AD Connect, vá a [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .
