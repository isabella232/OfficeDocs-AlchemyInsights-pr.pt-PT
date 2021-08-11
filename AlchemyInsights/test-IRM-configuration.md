---
title: Testar a Configuração de IRM para novas funcionalidades da OME
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12428"
- "9000078"
ms.openlocfilehash: 62697d6379ea6ab3c6af86d3bab752af560da7c1250e5ef6dd2a3eae8023a05e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "57812443"
---
# <a name="test-irm-configuration-for-new-ome-capabilities"></a>Testar a Configuração de IRM para novas funcionalidades da OME

Para verificar se o seu Microsoft 365 inquilino está configurado para utilizar novas funcionalidades da OME, execute os cmdlets seguintes enquanto estiver ligado [ao Exchange Online PowerShell:](/powershell/exchange/exchange-online-powershell)


1. Verifique a configuração da IRM do seu inquilino ao executar `Get-IRMConfiguration` o . Certifique-se de que estes valores estão definidos como **Verdadeiro:**
    
    **InternalLicensingEnabled**
    
    **ExternalLicensingEnabled**
    
    **AzureRMSLicensingEnabled**

2. Ao utilizar o seu domínio, endereço do remetente e destinatário, execute `Test-IRMConfiguration` . Se o teste não passar, investigue a sua configuração de IRM.

Para mais informações sobre como verificar a configuração da IRM, consulte Verificar a nova [configuração da OME no Exchange Online PowerShell.](/microsoft-365/compliance/set-up-new-message-encryption-capabilities#verify-new-ome-configuration-in-exchange-online-powershell)