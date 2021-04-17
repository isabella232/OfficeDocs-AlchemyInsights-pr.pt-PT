---
title: Eventos de calendário em falta ou não atualização
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10932"
- "9001435"
ms.openlocfilehash: b114411d6285a68a41bbcbf64151c212ee2cf661
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51837384"
---
# <a name="calendar-events-missing-or-not-updating"></a>Eventos de calendário em falta ou não atualização

Se faltam ou não atualizar os itens do calendário, comece por olhar para a contagem de artigos nas propriedades da pasta Do Calendário no Outlook: 

1. Clique com o botão direito na pasta **do calendário** do utilizador afetado e, em seguida, selecione **Propriedades**.

1. Selecione o separador **Sincronização.**

Se a contagem de artigos não for a mesma entre a pasta Servidor e a Pasta Offline:

1.  Realce a pasta **Calendário.**

1.  Vá ao  / separador Enviar **Receber** e, em seguida, selecione ''Atualizar Pasta' (Enviar) e, em seguida, selecione **' 'Actualizar' (Enviar)** e, em seguida,

Se o seu calendário ainda não estiver a atualizar ou faltar eventos, descarregue a Ferramenta de Verificação de Calendários para Perspetivas a partir do [centro de descarregamento](https://www.microsoft.com/download/details.aspx?id=28786)da Microsoft . Determine se existem mais de 5000 itens na pasta do calendário, uma vez que isso pode causar sintomas como reuniões de calendário não atualizadas ou erros de reunião. 

Para obter mais informações, consulte [os problemas de desempenho do Outlook quando há demasiados itens ou pastas num modo em cache .ost ou .pst file](https://docs.microsoft.com/outlook/troubleshoot/performance/performance-issues-if-too-many-items-or-folders).