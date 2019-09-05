---
title: A optimização Online do SharePoint
ms.author: pebaum
author: Techwriter40
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: d9e1400697b1e6435fea78703d2ecadc6733a57f
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/04/2019
ms.locfileid: "36751899"
---
# <a name="sharepoint-online-throttling"></a>A optimização Online do SharePoint

Os utilizadores poderão receber um 503 servidor estiver ocupado erro quando tentar navegar para sites SharePoint ou OneDrive. 

Este erro pode ser causado pelo estreitamento dentro do serviço SharePoint. SharePoint Online utiliza optimização para manter um óptimo desempenho e fiabilidade do serviço Online do SharePoint. Limites de estreitamento o número de acções do utilizador ou em simultâneo chamadas (por script ou código) para impedir a utilização excessiva de recursos. Se é limitada, 99% de tempo deve-se a código personalizado.

Para mais informações sobre optimização [evitar obter limitada ou bloqueado no SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online), consulte.

Se acha que este erro está relacionado com o estreitamento, pode verificar se existe manutenção activa que ocorram no seu tenant navegando para o [Centro de mensagens](https://portal.office.com/adminportal/home#/MessageCenter).

 Finalmente, certifique-se de que visitar a página de [Estado de funcionamento do serviço](https://portal.office.com/adminportal/home#/servicehealth) para verificar a existência de quaisquer avisos/incidentes que pode estar a ocorrer.

