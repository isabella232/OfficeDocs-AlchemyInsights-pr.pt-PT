---
title: Nenhum resultado devolvido durante a Pesquisa/Exportação de Conteúdos
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7463"
ms.openlocfilehash: 8786f11f170edb151879235e19caa38b50f3f06e
ms.sourcegitcommit: 3d662e1a1440ba74b5347896347d03bb8c8f3af5
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/22/2020
ms.locfileid: "49727234"
---
# <a name="no-results-returned-during-content-searchexport"></a>Nenhum resultado devolvido durante a Pesquisa/Exportação de Conteúdos

Se estiver a ter problemas com os seguintes cenários eDiscovery:

- Pesquisa/Exportação de conteúdos não devolve dados ou dados inesperados
- falha na pesquisa ou exportação de eDiscovery

Isto pode dever-se a certos filtros de segurança de conformidade que foram configurados por um administrador específico e não foram comunicados a todos os Administradores.

Para resolver isto, verifique se existem filtros de segurança de conformidade que possam estar a causar estes problemas:

1. Ligue-se ao Centro de Segurança e Conformidade Powershell
2. Executar os seguintes comandos:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

Para obter informações adicionais sobre filtros de segurança de conformidade, consulte [permissões de filtragem para pesquisa de conteúdo](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
