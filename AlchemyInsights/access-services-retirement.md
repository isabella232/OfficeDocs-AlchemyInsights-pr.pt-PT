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
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/15/2019
ms.locfileid: "36747795"
---
# <a name="access-services-retirement"></a>Aposentadoria dos serviços de acesso

Como anunciamos originalmente em MC97576, em março de 2017, e continuamos a se comunicar no ano passado, os Serviços de Acesso estão sendo aposentados do Office 365. A próxima fase desse processo será a remoção dos bancos de dados da Access Web que usam as listas do SharePoint como armazenamento de dados subjacente.

**Como isso me afeta?**

A partir de junho de 2019, vamos parar a criação de novos bancos de dados de acesso no SharePoint Online e encerrar o serviço e quaisquer aplicativos restantes até abril de 2020.

**O que preciso fazer para me preparar para essa mudança?**

Nós encorajamos você a criar um plano de transição para os bancos de dados da web Access da sua organização. Os administradores podem usar o scanner de [aplicativos SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) para obter um inventário dos aplicativos de acesso que os sites estão usando.

Existem várias maneiras de migrar dados de bancos de dados da web access:

- Importação para um banco de dados de acesso local (. ACCDB) ou para um arquivo Excel.
- Também recomendamos explorar o Microsoft PowerApps como uma plataforma alternativa para criar soluções de negócios sem código para dispositivos web e móveis.