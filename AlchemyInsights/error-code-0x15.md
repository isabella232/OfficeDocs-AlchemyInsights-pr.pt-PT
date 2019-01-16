---
title: Código de erro 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Se estiver a receber um erro ao activar o Office 2013 em implementações de serviços de ambiente de trabalho remoto (RDS), considere a activação ADAL editando o registo.
ms.openlocfilehash: 89f9270169e13fd7706f7826c624ef8ae4d47b3f
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/15/2019
ms.locfileid: "28305808"
---
Se estiver a receber um erro ao activar o Office 2013 em implementações de serviços de ambiente de trabalho remoto (RDS), considere a activação ADAL editando o registo. 
  
|**Chave de registo**|**Tipo**|**Value**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |
   
Para mais informações, consulte [Activar autenticação moderna para 2013 do Office em dispositivos do Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL está activado por predefinição no Office 365 ProPlus e de 2016 Office. > Serviços de ambiente de trabalho remoto (RDS) era anteriormente chamado dos serviços de Terminal. 
  

