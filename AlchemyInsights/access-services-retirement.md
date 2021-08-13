---
title: Aposentação dos serviços do Access
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
ms.openlocfilehash: 32da879de230dc0ed99563ad881ab5b2479b8453933a127961a26d619e108ab9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53938706"
---
# <a name="access-services-retirement"></a>Aposentação dos serviços do Access

Tal como anunciámos originalmente no MC97576, em março de 2017, continuação da comunicação ao longo do último Serviços do Access vai ser descontinuada. A próxima fase neste processo será a remoção das Bases de Dados Web do Access que utilizam as listas do SharePoint como o seu armazenamento de dados sub base.

**Como é que isto me afeta?**

A partir de junho de 2019, iremos interromper a criação de novas bases de dados do Access no SharePoint Online e encerrar o serviço e todas as aplicações restantes até abril de 2020.

**O que preciso de fazer para me preparar para esta alteração?**

Aconselhamo-lo a criar um plano de transição para as bases de dados Web do Access da sua organização. Os administradores podem utilizar o scanner de aplicações do [SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) para obter um inventário das aplicações do Access que os sites estão a utilizar.

Existem várias formas de migrar dados de bases de dados Web do Access:

- Importar para uma base de dados local do Access (. ACCDB) ou para um Excel ficheiro.
- Também recomendamos que explore este Microsoft PowerApps como uma plataforma alternativa para criar soluções empresariais sem código para web e dispositivos móveis.