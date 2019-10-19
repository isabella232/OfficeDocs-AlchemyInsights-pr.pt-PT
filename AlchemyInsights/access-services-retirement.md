---
title: Aposentadoria dos serviços de acesso
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 197366882468ebc87fc26f2fe2733371790d1871
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/18/2019
ms.locfileid: "36747795"
---
# <a name="access-services-retirement"></a>Aposentadoria dos serviços de acesso

Como originalmente anunciado no MC97576, em março de 2017, e continuou a se comunicar ao longo do ano passado, os serviços de acesso estão sendo retirados do Office 365. A próxima fase nesse processo será a remoção de bancos de dados da Web do Access que usam listas do SharePoint como seu armazenamento de dados subjacente.

**Como isso me afeta?**

A partir de junho 2019, vamos parar a criação de novos bancos de dados do Access no SharePoint Online e encerrar o serviço e quaisquer aplicativos restantes até abril de 2020.

**O que preciso fazer para me preparar para essa mudança?**

Incentivamos você a criar um plano de transição para os bancos de dados da Web do Access da sua organização. Os administradores podem usar o [scanner de aplicativo do SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) para obter um inventário dos aplicativos do Access que os sites estão usando.

Há várias maneiras de migrar dados do Access Web databases:

- Importando para um banco de dados do Access local (. ACCDB) ou para um arquivo do Excel.
- Também recomendamos explorar o Microsoft PowerApps como uma plataforma alternativa para criar soluções de negócios sem código para dispositivos móveis e da Web.