---
title: Ferramenta de exportação da Deteção de Tempo
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
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: f7b7e1ae4f1f686fa510403d398c4ff750dbadb9065b8d63701a927eeac52d9b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101313"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Não consegue instalar ou executar a Ferramenta de Exportação da Deteção de Segurança?

Se não conseguir instalar ou executar a Ferramenta de Exportação da Deteção de Dados Estadutivos para transferir os resultados da pesquisa, verifique o seguinte:
  
- O computador que está a utilizar cumpre estes pré-requisitos:

  - Versões de 32 bits ou de 64 bits do Windows 7 e versões posteriores

  - Microsoft .NET Framework 4.7

  - Um browser suportado:

  - Microsoft Edge

    Ou

  - Internet Explorer 10 e versões posteriores

    Outros browsers, como o Google Chrome e o Mozilla Firefox, não são suportados.

- A sua organização pode ligar ao ponto final no Azure, que é **\* .blob.core.windows.net** (o postal representa um identificador exclusivo para a sua tarefa de exportação).

- A função de Exportação é-lhe atribuída no Centro de Conformidade Microsoft 365 &amp; de Conformidade de Segurança. Por predefinição, esta função só está atribuída ao grupo de funções do Gestor da Deteção de Correio Online. Consulte [Atribuir permissões de Deteção de Email.](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions)

Para obter mais informações, consulte [Exportar resultados da Pesquisa de Conteúdos.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)

Se estiver a exportar mais de 100 mil caixas de correio, terá de utilizar o seguinte PowerShell para transferir os resultados de Exportar: Exportar resultados de mais de  [100K](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)caixas de correio.