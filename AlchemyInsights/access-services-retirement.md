---
title: Reforma de serviços de acesso
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 395dac6abf1562aa0da0b1d87eddd943affefc3f
ms.sourcegitcommit: b2c9202b94fa1ce73dbeb3e43b219ba07e46e7e3
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/14/2019
ms.locfileid: "33973940"
---
# <a name="access-services-retirement"></a>Reforma de serviços de acesso

Tal como foi originalmente anunciadas na MC97576, em Março de 2017 e continuaram a comunicar ao longo do ano passado, serviços de acesso estão a ser retirados do Office 365. A fase seguinte no processo será a remoção de bases de dados do Access Web que utilizam listas do SharePoint como seu armazenamento de dados subjacente.

## <a name="how-does-this-affect-me"></a>Isto afecta-me?

Iniciar de 2019 Junho, iremos parar a criação de novas bases de dados do Access no SharePoint Online e encerrar o serviço e as aplicações restantes até de Abril de 2020.

## <a name="what-do-i-need-to-do-to-prepare-for-this-change"></a>O que é necessário para preparar para que esta alteração?

Recomendamos que crie um plano de transição para a bases de dados web de acesso da sua organização. Admins pode utilizar o [scanner de aplicação de acesso ao SharePoint](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fgithub.com%2FSharePoint%2FPnP-Tools%2Ftree%2Fmaster%2FSolutions%2FSharePoint.AccessApp.Scanner&data=02%7C01%7Csalarson%40microsoft.com%7C0f8afc9cd02f45ac32d708d6d26c5b40%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636927760189423652&sdata=xH%2FPQdPyyGEUBiXfMwUAhBE4UmsuBa4JhFDZUbjUkZU%3D&reserved=0) para obter um inventário das aplicações de acesso a sites estão a utilizar. 

Existem várias formas para migrar dados de bases de dados do Access web:

- Importar uma base de dados local do Access (. ACCDB) ou para um ficheiro Excel.
- Recomendamos também explorar Microsoft PowerApps como uma plataforma alternativa para criar soluções de negócio sem código para a web e dispositivos móveis.