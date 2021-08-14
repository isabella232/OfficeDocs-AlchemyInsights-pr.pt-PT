---
title: Corrigir problemas de configuração do DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 5a613321ed79e657350ec4d19b1f07ac0a091b227a8268c793a10edd9990d41f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53945942"
---
# <a name="fix-dkim-setup-issues"></a>Corrigir problemas de configuração do DKIM

Se tiver problemas ao ativar o DKIM para o seu domínio personalizado, utilize os seguintes passos:

- A maioria dos problemas de configuração do DKIM estão relacionados com registos DNS incorretos. Verifique se o registo DKIM CNAME **(e não um** registo TXT) está formatado corretamente. Para obter mais informações, consulte este [tópico.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)

- Após criar ou atualizar os registos DKIM DNS no serviço de registo DNS do seu domínio (normalmente, a sua registo de domínios), aguarde até que os registos DNS se propaguem.

- Se não conseguir criar os registos DKIM DNS no centro de administração, pode substituir pelo seu domínio personalizado (por exemplo, contoso.com) e executar este comando no \<CustomDomain\> [Exchange Online PowerShell:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
