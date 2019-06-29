---
title: Reforma de serviços de acesso
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 5f171050479f34077f3dc155bec40437f86b84c0
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/28/2019
ms.locfileid: "35359369"
---
# <a name="access-services-retirement"></a>Reforma de serviços de acesso

Tal como foi originalmente anunciadas na MC97576, em Março de 2017 e continuaram a comunicar ao longo do ano passado, serviços de acesso estão a ser retirados do Office 365. A fase seguinte no processo será a remoção de bases de dados do Access Web que utilizam listas do SharePoint como seu armazenamento de dados subjacente.

**Isto afecta-me?**

Iniciar de 2019 Junho, iremos parar a criação de novas bases de dados do Access no SharePoint Online e encerrar o serviço e as aplicações restantes até de Abril de 2020.

**O que é necessário para preparar para que esta alteração?**

Recomendamos que crie um plano de transição para a bases de dados web de acesso da sua organização. Admins pode utilizar o [scanner de aplicação de acesso ao SharePoint](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) para obter um inventário das aplicações de acesso a sites estão a utilizar.

Existem várias formas para migrar dados de bases de dados do Access web:

- Importar uma base de dados local do Access (. ACCDB) ou para um ficheiro Excel.
- Recomendamos também explorar Microsoft PowerApps como uma plataforma alternativa para criar soluções de negócio sem código para a web e dispositivos móveis.