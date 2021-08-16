---
title: Código de 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Se estiver a receber uma mensagem de erro durante a ativação da implementação do Office 2013 em Serviços de Ambiente de Trabalho Remoto (RDS), considere ativar a ADAL ao editar o registo.
ms.openlocfilehash: 247686bf26c11d07ed118bdb1ba190fc718e87cf140b88f79b8aa0b40c827b4d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54100773"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Erro durante a Office 2013 nos Serviços de Ambiente de Trabalho Remoto

Se estiver a receber uma mensagem de erro durante a ativação da implementação do Office 2013 em Serviços de Ambiente de Trabalho Remoto (RDS), considere ativar a ADAL ao editar o registo.
  
|**Chave de registo**|**Tipo**|**Valor**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Para obter mais informações, consulte [Ativar a Autenticação Moderna Office 2013 em Windows dispositivos](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  A ADAL está ativada por predefinição no Microsoft 365 Apps para Grandes Empresas e Office 2016. Os Serviços de Ambiente de Trabalho Remoto (RDS) eram anteriormente denominados Serviços de Terminal.
  