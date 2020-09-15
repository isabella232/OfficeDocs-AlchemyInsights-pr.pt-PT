---
title: Pesquisa de conteúdo Sem Resultados
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 1e90c403556a317ff810971ccfa4a91694fb1171
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680658"
---
# <a name="no-results-from-content-searchexports"></a>Sem resultados de Pesquisa/Exportações de Conteúdos

Problemas com a Pesquisa/Exportações de Conteúdo que não devolvam quaisquer dados podem dever-se a um certo Filtro de Segurança de Conformidade que foi configurado por um Administrador específico e não os comunicando a todos os Administradores.

Para resolver isto, verifique se existem filtros de segurança de conformidade que possam estar a causar isto:
1. Ligue-se ao Centro de Segurança e Conformidade Powershell
2. Executar os seguintes comandos:
<br>$org = "yourdomain.com"
<br>Obtém-ComplianceSecurityFilter - Organização $org