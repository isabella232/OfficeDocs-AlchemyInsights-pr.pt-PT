---
title: A questão do spooler de impressão está resolvida
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 53b1c9a8efa3cc978af8b602c8ed90430042186a
ms.sourcegitcommit: 4265a9e79db6c2a396aa80ec0ebd467bbaadf366
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/08/2020
ms.locfileid: "45088404"
---
# <a name="print-spooler-issue-is-resolved"></a>A questão do spooler de impressão está resolvida

Se o seu dispositivo foi atualizado com o Windows 10 **OS Build 19041.329**, pode ter observado um problema em que determinadas impressoras não conseguem imprimir. O spooler de impressão pode lançar um erro ou fechar inesperadamente ao tentar imprimir, e nenhuma saída vem da impressora afetada. Esta questão é resolvida em OS Build **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).  

**Investigação em curso**

O ficheiro do Serviço de Subsistema da Autoridade de Segurança Local (LSASS)** (Isass.exe) **pode falhar em alguns dispositivos com a mensagem de erro: "Um processo crítico do sistema, C:\WINDOWS\system32\Isass.exe, falhou com o código de estado c0000008. A máquina deve agora ser reiniciada".  **A Microsoft está a trabalhar numa resolução e irá fornecer uma atualização numa próxima versão.**

Para mais informações, consulte [os problemas conhecidos do Windows 10 Version 2004.](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc)