---
title: O erro de ligação subdatante foi fechado no SharePoint
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 04/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10802"
- "9006390"
ms.openlocfilehash: b64215b5b83ef1092eb58791e6dbb015b72d422d
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233437"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a>Erro "A ligação subcente foi fechada" no SharePoint

Se receber a mensagem de erro "A ligação subfeita foi fechada" no SharePoint, esta pode estar relacionada com a despreciação do TLS 1.0/1.1. Para mais informações, consulte estes artigos:

- [Preparando-se para o TLS 1.2 no Office 365 e Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365?view=o365-worldwide)

- [Os erros de autenticação ocorrem se o cliente não tiver suporte TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

Se os utilizadores estiverem Windows 7, certifique-se de que verificam [o TLS Cipher Suites no Windows 7.](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7)