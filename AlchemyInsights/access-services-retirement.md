---
title: Reforma dos serviços de acesso
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 977bd5887ef58b328463a9befcd6b47ac55f5a85
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687269"
---
# <a name="access-services-retirement"></a>Reforma dos serviços de acesso

Como inicialmente anunciamos no MC97576, em março de 2017, e continuamos a comunicar ao longo do ano passado os Serviços de Acesso estão a ser retirados. A próxima fase deste processo será a remoção de Bases de Dados Web de Acesso que utilizam as listas do SharePoint como armazenamento de dados subjacentes.

**Como é que isto me afeta?**

A partir de junho de 2019, vamos parar a criação de novas bases de dados de Acesso no SharePoint Online e encerrar o serviço e quaisquer aplicações restantes até abril de 2020.

**O que preciso fazer para me preparar para esta mudança?**

Encorajamo-lo a criar um plano de transição para as bases de dados web access da sua organização. Os administradores podem usar o scanner de [aplicações SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) para obter um inventário das aplicações access que os sites estão a usar.

Existem várias formas de migrar dados de bases de dados web do Access:

- Importando para uma base de dados de acesso local (. ACCDB) ou para um ficheiro Excel.
- Recomendamos também a exploração do Microsoft PowerApps como uma plataforma alternativa para criar soluções de negócio sem código para dispositivos web e móveis.