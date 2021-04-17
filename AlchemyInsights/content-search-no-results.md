---
title: Pesquisa de conteúdo Sem Resultados
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 0267286ca5967ee891e65343d49adf776f0322a6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816859"
---
# <a name="no-results-from-content-searchexports"></a>Sem resultados de Pesquisa/Exportações de Conteúdos

Problemas com a Pesquisa/Exportações de Conteúdo que não devolvam quaisquer dados podem dever-se a um certo Filtro de Segurança de Conformidade que foi configurado por um Administrador específico e não os comunicando a todos os Administradores.

Para resolver isto, verifique se existem filtros de segurança de conformidade que possam estar a causar isto:
1. Ligue-se ao Centro de Segurança e Conformidade Powershell
2. Executar os seguintes comandos:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter -Organização $org