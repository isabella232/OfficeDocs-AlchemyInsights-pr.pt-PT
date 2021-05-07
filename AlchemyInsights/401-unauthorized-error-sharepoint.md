---
title: 401 Erro não autorizado no SharePoint
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10935"
- "9001435"
ms.openlocfilehash: 6799b2112458a7ab3715c9b63e03c2c7ca3fe6be
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233519"
---
# <a name="401-unauthorized-error-in-sharepoint"></a>401 Erro não autorizado no SharePoint

Se receber o erro "(401) Não Autorizado" no SharePoint, este poderá estar relacionado com a preterição do TLS 1.0/1.1. Para obter mais informações, consulte:

[Preparando-se para o TLS 1.2 no Office 365 e Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

[Os erros de autenticação ocorrem se o cliente não tiver suporte TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

Se os utilizadores estiverem Windows 7, certifique-se de que verificam [o TLS Cipher Suites no Windows 7.](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7)