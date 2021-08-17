---
title: 932 Atualizar o AADConnect
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
ms.openlocfilehash: 9582f1f56e6730e35520b5d79bc245cd74bea0bf4db39b379a7cd133bafc16ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104823"
---
# <a name="upgrade-azure-ad-connect"></a>Atualizar o Azure AD Ligação

Por predefinição, a atualização automática está ativada para o Azure AD Ligação, o que ajuda a garantir que está a executar a versão mais recente. Para verificar as definições de atualização automática, utilize o cmdlet **Get-ADSyncAutoUpgrade** no Azure AD PowerShell. O cmdlet irá devolver um dos seguintes valores:

- **Ativado:** A atualização automática está ativada.

- **Desativada:** a atualização automática está desativada.

- **Suspenso**: O sistema já não é elegível para receber atualizações automáticas. Não pode configurar este valor; é definida pelo sistema.

Para obter mais informações, consulte [Atualização automática.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)

Para transferir a versão mais recente do Azure AD Ligação, vá para [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .
