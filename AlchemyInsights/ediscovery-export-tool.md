---
title: ferramenta de exportação eDiscovery
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
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: 67e59182a5053111a08f5fb2be814931a1aa815d
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277935"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Não pode instalar ou executar a ferramenta de exportação eDiscovery?

Se não conseguir instalar ou executar a Ferramenta de Exportação de eDiscovery para descarregar os resultados da pesquisa, verifique as seguintes coisas:
  
- O computador que está a usar cumpre estes requisitos:

  - Versões de 32 ou 64 bits do Windows 7 e versões posteriores

  - Microsoft .NET Framework 4.7

  - Um navegador suportado:

  - Microsoft Edge

    Ou

  - Versões 10 e posteriores do Internet Explorer

    Outros navegadores, como o Google Chrome e Mozilla Firefox, não são suportados.

- A sua organização pode ligar-se ao ponto final em Azure, que é ** \* .blob.core.windows.net** (o wildcard representa um identificador único para o seu trabalho de exportação).

- Foi-lhe atribuída a função de Exportação no Microsoft 365 Security &amp; Compliance Center. Por padrão, esta função é atribuída apenas ao grupo de funções eDiscovery Manager. Ver [Atribuir permissões eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).

Para obter mais informações, consulte [os resultados da Pesquisa de Conteúdos de Exportação.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)

Se estiver a exportar mais de 100mil caixas de correio, terá de utilizar o seguinte Powershell para descarregar os resultados [da Exportação: Exportar resultados de mais de 100mil caixas de correio.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)