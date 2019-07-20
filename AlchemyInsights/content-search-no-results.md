---
title: Não existem resultados de pesquisa de conteúdo
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 9f2c0273762f1a4a2b905487f461dc1d05db9209
ms.sourcegitcommit: 8f97342d8b46ab05f1e89018473caad9d35431df
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/19/2019
ms.locfileid: "35800522"
---
# <a name="no-results-from-content-searchexports"></a>Não existem resultados de conteúdo procura/exportações

Problemas com conteúdo procura/exportações não devolver quaisquer dados podem ser devido a certas filtro de segurança de conformidade que foi configurado por um administrador específico e não a comunicar a todos os Admins.

Para resolver este problema, verifique se existem quaisquer filtros de segurança de conformidade que poderá estar a causar este:
1. Ligar a segurança e conformidade Centro Powershell
2. Execute o commandlets do seguinte:
<br>$org = "seudomínio. com"
<br>Get-ComplianceSecurityFilter-$org de organização