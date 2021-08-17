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
ms.openlocfilehash: 8935f461aaf24cb100516311203ef642f5dbed931e472df944c1cd7e72a8cf4e
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/11/2021
ms.locfileid: "57890277"
---
# <a name="401-unauthorized-error-in-sharepoint"></a>401 Erro não autorizado no SharePoint

Se receber o erro "(401) Não Autorizado" no SharePoint, este poderá estar relacionado com a preterição do TLS 1.0/1.1. Para obter mais informações, consulte:

- [Preparando-se para o TLS 1.2 no Office 365 e Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Os erros de autenticação ocorrem se o cliente não tiver suporte TLS 1.2](https://docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Atualização para ativar o TLS 1.1 e o TLS 1.2 como protocolos seguros predefinido no WinHTTP no Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Se os utilizadores estiverem Windows 7, certifique-se de que verificam [os Conjuntos de Cipher Suites TLS no Windows 7.](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7)