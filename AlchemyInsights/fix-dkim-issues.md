---
title: Corrigir problemas de configuração dKIM
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
ms.openlocfilehash: d725eb0d46dcbf1b5b6d77ca9f59fcafa5298bf1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43717573"
---
# <a name="fix-dkim-setup-issues"></a>Corrigir problemas de configuração dKIM

Se tiver problemas que permitem o DKIM para o seu domínio personalizado, utilize os seguintes passos:

- A maioria dos problemas de configuração do DKIM estão relacionados com registos DNS incorretos. Verifique se o registo DKIM CNAME **(não** um disco TXT) está formatado corretamente. Para mais informações, consulte este [tema.](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365)

- Depois de criar ou atualizar os seus registos DKIM DNS no serviço de hospedagem DNS para o seu domínio (normalmente, o seu registo de domínio), aguarde que os registos dNS se propaguem.

- Se não conseguir criar os registos DNS DNS no \<centro\> de administração, pode substituir o CustomDomain pelo seu domínio `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`personalizado (por exemplo, contoso.com) e executar este comando no Exchange Online [PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): .
