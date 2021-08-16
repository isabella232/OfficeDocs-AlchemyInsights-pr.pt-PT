---
title: Sem Resultados da Pesquisa de Conteúdos
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
ms.openlocfilehash: b53534dd0666fa64e692910aa6800abab30169a97fbe567c815ce6b948381a63
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058013"
---
# <a name="no-results-from-content-searchexports"></a>Nenhum resultado da Pesquisa/Exportações de Conteúdo

Os problemas com a Pesquisa/Exportações de Conteúdos não devolvem quaisquer dados podem ser devido a determinado Filtro de Segurança de Conformidade que foi configurado por um Administrador específico e não ao communicá-lo a todos os Administradores.

Para resolver esta situação, verifique se existem Filtros de Segurança de Conformidade que possam estar a causar este problema:
1. Ligação ao PowerShell do Centro de Conformidade e Segurança
2. Execute os seguintes comandos:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter -Organização $org