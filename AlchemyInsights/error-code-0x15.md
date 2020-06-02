---
title: Código de erro 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Se estiver a receber um erro ao ativar o Office 2013 nas implementações de Serviços de Ambiente de Trabalho Remoto (RDS), considere ativar o ADAL editando o registo.
ms.openlocfilehash: 468d13e59602cf173ed2e17af44c66babfc28703
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506857"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Erro durante a ativação Do Office 2013 em Serviços de Ambiente de Trabalho Remoto

Se estiver a receber um erro ao ativar o Office 2013 nas implementações de Serviços de Ambiente de Trabalho Remoto (RDS), considere ativar o ADAL editando o registo.
  
|**Chave de registo**|**Tipo**|**Valor**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identidade\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Para obter mais informações, consulte [Ativar a Autenticação Moderna do Office 2013 em dispositivos Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  O ADAL está ativado por padrão nas Aplicações Microsoft 365 para empresas e Office 2016. Serviços remotos de desktop (RDS) foi anteriormente nomeado Terminal Services.
  