---
title: 1490-resolução de problemas-falhas na descoberta
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1490"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: ff28f96d64ec14980e9a47b630246b394faf4610
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277845"
---
# <a name="troubleshoot-content-search-errors"></a>Resolução de problemas Erros de pesquisa de conteúdo

Está a ter problemas com a Pesquisa de Conteúdo ou com falhas quando exporta resultados de pesquisa?

Por exemplo, está a receber o seguinte ao fazer pesquisas?

- Erros CS008 ou CS012

- Erros ocupados/tempoout do servidor

- Erro de aplicação ocorreu

Ou quando pesquisar ou exportar resulta de um grande número de caixas de correio (mais de 100.000 caixas de correio), está a obter erros de exportação?

Para este tipo de erros, recandiduça a procura das localizações de conteúdo que falharam. Consulte  [este artigo](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) para mais informações.

Se estiver a exportar mais de 100mil caixas de correio, terá de utilizar o seguinte Powershell para descarregar os resultados [da Exportação: Exportar resultados de mais de 100mil caixas de correio.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)
