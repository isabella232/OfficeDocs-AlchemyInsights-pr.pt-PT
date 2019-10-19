---
title: ferramenta de exportação de eDiscovery
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 8/3/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: 5a54344d43d16c77d440768aa1c87489edf10ca0
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/18/2019
ms.locfileid: "36736336"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Não é possível instalar ou executar a ferramenta de exportação de eDiscovery?

Se você não conseguir instalar ou executar a ferramenta de exportação de eDiscovery do Office 365 para baixar os resultados da pesquisa, verifique as seguintes coisas:
  
- O computador que você está usando atende a esses pré-requisitos:

  - 32-ou 64-bit versões do Windows 7 e versões posteriores

  - Microsoft .NET Framework 4,7

  - Um navegador suportado:

  - Borda da Microsoft

    Ou

  - Internet Explorer 10 e versões posteriores

    Outros navegadores, como o Google Chrome e o Mozilla Firefox, não são suportados.

- Sua organização pode se conectar ao ponto de extremidade no Azure, que é ** \*. blob.Core.Windows.net** (o curinga representa um identificador exclusivo para seu trabalho de exportação).

- É atribuída a função exportar no centro de conformidade de segurança &amp; do Office 365. Por padrão, essa função só é atribuída ao grupo de função Gerenciador de eDiscovery. Consulte [atribuir permissões de eDiscovery](https://docs.microsoft.com/office365/securitycompliance/assign-ediscovery-permissions).

Para obter mais informações, consulte [Exportar resultados da pesquisa de conteúdo](https://docs.microsoft.com/office365/securitycompliance/export-search-results).
  