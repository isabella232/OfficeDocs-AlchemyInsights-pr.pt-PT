---
title: Não foram devolvidos resultados durante a Pesquisa/Exportação de Conteúdos
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
ms.openlocfilehash: 5c04364f98dccbcad0f011df866f137d79c166ad3839b408d6be447d50a87ac3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101277"
---
# <a name="no-results-returned-during-content-searchexport"></a>Não foram devolvidos resultados durante a Pesquisa/Exportação de Conteúdos

Se estiver a ter problemas com os seguintes cenários de Deteção de Problemas:

- A Pesquisa/Exportação de Conteúdos não devolve dados ou dados inesperados
- A Pesquisa ou Exportação da Deteção de Emails falha

Isto pode ser devido a determinados Filtros de Segurança de Conformidade que foram configurados por um Administrador específico e que não foram comunicados a todos os Administradores.

Para resolver esta situação, verifique se existem Filtros de Segurança de Conformidade que possam estar a causar estes problemas:

1. Ligação ao PowerShell do Centro de Conformidade e Segurança
2. Execute os seguintes comandos:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

Para obter informações adicionais sobre os Filtros de Segurança de Conformidade, consulte [Filtragem de Permissões para a Pesquisa de Conteúdos](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
