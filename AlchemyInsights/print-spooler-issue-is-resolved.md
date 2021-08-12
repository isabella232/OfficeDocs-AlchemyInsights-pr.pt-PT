---
title: O problema do spooler de impressão foi resolvido
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 73ff86928c043dd41f49d456d30c2fcf7947bd4cb304d0456c634d4fa5808239
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53911349"
---
# <a name="print-spooler-issue-is-resolved"></a>O problema do spooler de impressão foi resolvido

Se o seu dispositivo tiver sido atualizado com a Comtrução **19041.329** do Windows 10 SO, poderá ter observado um problema em que determinadas impressoras não são impressas.   O spooler de impressão poderá detetar um erro ou fechar-se inesperadamente ao tentar imprimir e não será devolva nenhum resultado da impressora afetada. Este problema foi resolvido na Comtrução do SO **19041.331,** [KB4567523.](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523)  

**Investigação em curso**

O ficheiro de Serviço de Subssistema de Autoridade de Segurança Local (LSASS)**(Isass.exe)** poderá falhar em alguns dispositivos com a mensagem de erro "Um processo de sistema crítico, C:\WINDOWS\system32\Isass.exe, falhou com o código de estado c0000008. O aparelho tem de ser reiniciado".  **A Microsoft está a trabalhar numa resolução e fornecerá uma atualização num lançamento futuro.**

Para obter mais informações, consulte o Windows 10 de problemas conhecidos da Versão [2004.](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc)