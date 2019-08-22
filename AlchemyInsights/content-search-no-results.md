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
ms.openlocfilehash: 09cdbc3cb0465e0e0bc08872c49e283081ad3e92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36516790"
---
# <a name="no-results-from-content-searchexports"></a>Não existem resultados de conteúdo procura/exportações

Problemas com conteúdo procura/exportações não devolver quaisquer dados podem ser devido a certas filtro de segurança de conformidade que foi configurado por um administrador específico e não a comunicar a todos os Admins.

Para resolver este problema, verifique se existem quaisquer filtros de segurança de conformidade que poderá estar a causar este:
1. Ligar a segurança e conformidade Centro Powershell
2. Execute o commandlets do seguinte:
<br>$org = "seudomínio. com"
<br>Get-ComplianceSecurityFilter-$org de organização