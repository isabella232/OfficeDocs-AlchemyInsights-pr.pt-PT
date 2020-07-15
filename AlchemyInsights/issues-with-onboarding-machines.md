---
title: Problemas com máquinas de embarque
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 19b516dc21472e2c80a8b9046f802b329d15e4d6
ms.sourcegitcommit: 45c2aaeee58c0be466b76c7f0cd71e796d3c8f76
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/15/2020
ms.locfileid: "45141657"
---
# <a name="issues-with-onboarding-machines"></a>Problemas com máquinas de embarque

Pode ter problemas com máquinas de bordo para o serviço MDATP. Se conseguir aceder à máquina do utilizador final, siga estes passos:

1. Descarregue a ferramenta de diagnóstico [de Análise de Conectividade do Cliente.](https://aka.ms/mdatpanalyzer)
2. Extrair e executar MDATPAnalyzer.cmd.
3. Localizar o registo de diagnóstico na pasta chamada MDATPClientAnalyzerResult, a mesma pasta onde a ferramenta Analyzer é descarregada.
4. Reveja o ficheiro de registo, MDATPClientAnalyzer.txt, para encontrar problemas de configuração de conectividade ou procuração de internet.