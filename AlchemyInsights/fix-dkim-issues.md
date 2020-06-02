---
title: Corrigir problemas de configuração DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 8195b0e3fada6da033b2d95b1fc6600e7fa3341e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506785"
---
# <a name="fix-dkim-setup-issues"></a>Corrigir problemas de configuração DKIM

Se sentir problemas que permitam ao DKIM para o seu domínio personalizado, utilize os seguintes passos:

- A maioria dos problemas de configuração do DKIM estão relacionados com registos DNS incorretos. Verifique se o registo DKIM CNAME **(não** um registo TXT) está formatado corretamente. Para mais informações, consulte este [tópico.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)

- Depois de criar ou atualizar os registos DKIM DNS no serviço de hospedagem DNS para o seu domínio (normalmente, o seu registo de domínio), aguarde que os registos DNS se propaguem.

- Se não conseguir criar os registos DKIM DNS no centro de administração, pode \<CustomDomain\> substituir-se pelo seu domínio personalizado (por exemplo, contoso.com) e executar este comando em [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
