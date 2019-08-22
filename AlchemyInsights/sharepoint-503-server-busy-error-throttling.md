---
title: A optimização Online do SharePoint
ms.author: kirks
author: Techwriter40
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: c7881c0c7331e0aa74fcc439f52157bb75a56160
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36559852"
---
# <a name="sharepoint-online-throttling"></a>A optimização Online do SharePoint

Os utilizadores poderão receber um 503 servidor estiver ocupado erro quando tentar navegar para sites SharePoint ou OneDrive. 

Este erro pode ser causado pelo estreitamento dentro do serviço SharePoint. SharePoint Online utiliza optimização para manter um óptimo desempenho e fiabilidade do serviço Online do SharePoint. Limites de estreitamento o número de acções do utilizador ou em simultâneo chamadas (por script ou código) para impedir a utilização excessiva de recursos. Se é limitada, 99% de tempo deve-se a código personalizado.

Para mais informações sobre optimização [evitar obter limitada ou bloqueado no SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online), consulte.

Se acha que este erro está relacionado com o estreitamento, pode verificar se existe manutenção activa que ocorram no seu tenant navegando para o [Centro de mensagens](https://portal.office.com/adminportal/home#/MessageCenter).

 Finalmente, certifique-se de que visitar a página de [Estado de funcionamento do serviço](https://portal.office.com/adminportal/home#/servicehealth) para verificar a existência de quaisquer avisos/incidentes que pode estar a ocorrer.

