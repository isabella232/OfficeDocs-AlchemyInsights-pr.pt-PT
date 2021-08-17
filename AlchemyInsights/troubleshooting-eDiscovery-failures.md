---
title: 1490-troubleshooting-eDiscovery-failures
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
ms.openlocfilehash: 7b819b9bb18b5c0a635e708eccc0f23271267874707e5f3a7d41b633a05f2822
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105579"
---
# <a name="troubleshoot-content-search-errors"></a>Remoção de erros de Pesquisa de Conteúdos

Está a ter problemas com a Pesquisa de Conteúdos ou está a obter falhas ao exportar os resultados da pesquisa?

Por exemplo, está a receber o seguinte ao executar pesquisas?

- Erros CS008 ou CS012

- Erros de ocupado/tempo de insu remoção do servidor

- Ocorreu um erro de aplicação

Ou, ao procurar ou exportar resultados de um grande número de caixas de correio (mais de 100.000 caixas de correio), está a obter erros de exportação?

Para estes tipos de erros, procure as localizações de conteúdo que falharam. Consulte  [este artigo](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) para obter mais informações.

Se estiver a exportar mais de 100 mil caixas de correio, terá de utilizar o seguinte PowerShell para transferir os resultados de Exportar: Exportar resultados de mais de  [100K](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)caixas de correio.
