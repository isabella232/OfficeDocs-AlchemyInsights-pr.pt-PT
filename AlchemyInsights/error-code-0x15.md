---
title: Código de erro 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Se estiver a receber um erro ao activar o Office 2013 em implementações de serviços de ambiente de trabalho remoto (RDS), considere a activação ADAL editando o registo.
ms.openlocfilehash: e2249d8ebbd2313c64dda5656a3243fa76d97a9a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/28/2019
ms.locfileid: "35388256"
---
Se estiver a receber um erro ao activar o Office 2013 em implementações de serviços de ambiente de trabalho remoto (RDS), considere a activação ADAL editando o registo.
  
|**Chave de registo**|**Tipo**|**Valor**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Para mais informações, consulte [Activar autenticação moderna para 2013 do Office em dispositivos do Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL está activado por predefinição no Office 365 ProPlus e de 2016 Office. > serviços de ambiente de trabalho remoto (RDS) era anteriormente chamado dos serviços de Terminal.
  