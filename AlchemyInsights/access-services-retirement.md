---
title: Aposentadoria de serviços de acesso
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 943066d5ac76c0630554ee724bbab9a94086fae4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698693"
---
# <a name="access-services-retirement"></a>Aposentadoria de serviços de acesso

Como inicialmente anunciado no MC97576, em março de 2017, e continuamos a comunicar ao longo do ano passado, os Serviços de Acesso estão a ser reformados. A próxima fase deste processo será a remoção de Bases de Dados Web de Acesso que utilizam as listas do SharePoint como o seu armazenamento de dados subjacente.

**Como é que isto me afeta?**

A partir de junho de 2019, vamos parar a criação de novas bases de dados de Acesso no SharePoint Online e encerrar o serviço e quaisquer aplicações restantes até abril de 2020.

**O que preciso de fazer para me preparar para esta mudança?**

Encorajamo-lo a criar um plano de transição para as bases de dados web access da sua organização. Os administradores podem usar o scanner de [aplicações SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) para obter um inventário das aplicações Access que os sites estão a usar.

Existem várias formas de migrar os dados das bases de dados do Access Web:

- Importando para uma base de dados de acesso local (. ACCDB) ou para um ficheiro Excel.
- Recomendamos também explorar o Microsoft PowerApps como uma plataforma alternativa para criar soluções de negócio sem código para dispositivos web e móveis.