---
title: Problemas com o SharePoint em Windows 7 máquinas
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9006484"
- "11070"
ms.openlocfilehash: 787f0e713cc95b590bc494868d5098a25131ac56
ms.sourcegitcommit: d33ab8c73d8af51da782094fb8f8abf7626f4df3
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/28/2021
ms.locfileid: "52125514"
---
# <a name="issues-with-sharepoint-on-windows-7-machines"></a>Problemas com o SharePoint em Windows 7 máquinas

Se receber erros em Windows 7 máquinas a trabalhar no SharePoint ou no OneDrive, estes podem estar relacionados com a depreciação do TLS 1.0/1.1. Para mais informações, consulte:

- [Preparando-se para o TLS 1.2 no Office 365 e Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- Windows 7 SP1/Windows 8 têm de ter o TLS1.2 ativado. Para obter mais informações, consulte Ocorrem erros de autenticação quando o cliente não tem suporte [TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- Instale a atualização KB3140245 e crie o valor de registo. Para obter mais informações, consulte Update [to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

- Windows 7 SP1/Windows 8 têm de garantir que os conjuntos de aplicações cipher TLS mais recentes estão instalados. Para obter mais informações, consulte [o Aviso de Segurança da Microsoft 3042058.](https://docs.microsoft.com/security-updates/SecurityAdvisories/2015/3042058) 


