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
ms.openlocfilehash: 101c0ba90d2bec6b1684fd63645ba2f8f89783ad5bfdf0efe739d31dfd951f66
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044423"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a>Erro "A ligação subcente foi fechada" no SharePoint

Se receber a mensagem de erro "A ligação subfeita foi fechada" no SharePoint, esta pode estar relacionada com a despreciação do TLS 1.0/1.1. Para mais informações, consulte estes artigos:

- [Preparando-se para o TLS 1.2 no Office 365 e Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Os erros de autenticação ocorrem se o cliente não tiver suporte TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Atualização para ativar o TLS 1.1 e o TLS 1.2 como protocolos seguros predefinido no WinHTTP no Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Se os utilizadores estiverem Windows 7, certifique-se de que verificam [o TLS Cipher Suites no Windows 7.](/windows/win32/secauthn/tls-cipher-suites-in-windows-7)