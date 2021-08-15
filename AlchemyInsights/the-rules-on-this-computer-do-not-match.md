---
title: 'Erro: as regras neste computador não correspondem'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: b77573e9d94195e1f0ef4a1566c45a30d53b7e68e502aeb834e2ca5b9e6c5c76
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53981124"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>Erro: as regras neste computador não correspondem

Para ver o estado atualizado deste problema conhecido, consulte As regras neste computador [não correspondem às do Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)

A Outlook Equipa de Equipa implementou uma correção na Complicação 12928.10000. A correção já está no Insider Fast e será via Via de Distribuição Mensal no final de junho de 2020. Assim que tiver a comtrução corrigida, poderá ser-lhe pedido "Quais são as regras que pretende manter" uma última vez. Selecionar Servidor quando lhe for pedido, volte ao Outlook e volte a ativar todas as regras que foram desativadas.

Até a correção estar disponível, utilize a seguinte solução:

**Maneira de resolver o** problema: Em relatórios recentes, o problema ocorreu em pessoas que apenas criaram regras de cliente no Outlook ambiente de trabalho. Se continuar a detetar o problema, considere eliminar as regras e, em seguida, crie e edite regras apenas no OWA (Outlook Web App) até que o problema seja resolvido.

Se não conseguir eliminar as regras manualmente, pode executar um comando Outlook quando iniciar o Outlook ao executar Outlook.exe /cleanrules. Esta ação irá eliminar as regras do cliente e do servidor. Esta ação irá eliminar todas as regras de todas as contas no Outlook Perfil. Este comando está ainda documentado no artigo Comutador da linha de comandos.

