---
title: 1336 Pasta RecoveryAbleItems está cheia
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: fb10b792981040bdcf4661b8aff30733c2438212
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720263"
---
# <a name="the-recoverable-items-folder-is-full"></a>A pasta de Itens Recuperáveis está cheia

Para trocar caixas de correio online, o limite de armazenamento predefinido para a pasta "Itens Recuperáveis" é de 30 GB. O limite de armazenamento da pasta Itens Recuperáveis é automaticamente aumentado para 100 GB se a caixa de correio for colocada em Litigation Hold, eDiscovery hold ou for atribuída a uma política de retenção.

Quando a pasta "Itens Recuperáveis" atinge o limite de armazenamento, a funcionalidade da caixa de correio é afetada das seguintes formas:

- O utilizador não pode apagar artigos da caixa de correio.

- O Assistente de Pasta Gerida não pode eliminar itens com base na etiqueta de retenção ou nas definições de pasta geridas.

- Para caixas de correio que tenham a Recuperação do Item Único ativada ou colocadas em espera, o processo de proteção da página copy-on-write não pode manter versões de itens editados pelo utilizador.

- Para caixas de correio que tenham registo de auditoria de caixa de correio ativado, nenhuma entrada de registo de auditoria de caixa de correio pode ser guardada na subpasta de Auditorias na pasta Itens Recuperáveis.

Para caixas de correio que não estejam em espera, os administradores podem usar o `Search-Mailbox -SearchDumpsterOnly -DeleteContent` comando no Exchange Online PowerShell para eliminar itens na pasta Itens Recuperáveis. For more information, see the following topics:

- [Pesquisar e eliminar mensagens](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)

- [Caixa de pesquisa-correio](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

Para as caixas de correio que estão em espera, os administradores têm de remover o porão antes de poderem apagar itens da pasta Itens Recuperáveis. Para mais informações, consulte Apagar itens na pasta de [Itens Recuperáveis das caixas de correio baseadas na nuvem em espera](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

Para ajudar a evitar que a pasta De Itens Recuperáveis fique cheia, os administradores podem aumentar o limite de armazenamento da pasta De Itens Recuperáveis para caixas de correio em espera e configurar uma política de retenção de caixas de correio que transfere itens da pasta De Itens Recuperáveis para a caixa de correio de arquivo do utilizador. Ver Aumentar a quota de [itens recuperáveis para caixas de correio em espera](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
