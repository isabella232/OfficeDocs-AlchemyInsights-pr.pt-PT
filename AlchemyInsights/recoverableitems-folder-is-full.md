---
title: 1336 A pasta RecoverableItems está cheia
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 6ae608b776332402fe333315f5e4ff6072b0a651
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741278"
---
# <a name="the-recoverable-items-folder-is-full"></a>A pasta de Itens Recuperáveis está cheia

Para caixas de correio Exchange Online, o limite de armazenamento predefinido para a pasta Itens Recuperáveis é de 30 GB. O limite de armazenamento da pasta Itens Recuperáveis é automaticamente aumentado para 100 GB se a caixa de correio for colocada em Hold de Litígio, porão eDiscovery ou for atribuída a uma política de retenção.

Quando a pasta Itens Recuperáveis atinge o limite de armazenamento, a funcionalidade da caixa de correio é afetada das seguintes formas:

- O utilizador não pode eliminar os itens da caixa de correio.

- O Assistente de Pasta Gerida não pode eliminar itens baseados na etiqueta de retenção ou nas definições de pasta geridas.

- Para caixas de correio que tenham a Recuperação de Item Único ativada ou colocadas em espera, o processo de proteção da página de cópia na escrita não consegue manter versões de itens editados pelo utilizador.

- Para caixas de correio que tenham registo de auditoria de caixa de correio ativado, não podem ser guardadas entradas de registo de auditoria na sub-dobragem de Auditorias na pasta Itens Recuperáveis.

Para caixas de correio que não estejam em espera, os administradores podem utilizar o `Search-Mailbox -SearchDumpsterOnly -DeleteContent` comando em Exchange Online PowerShell para eliminar itens na pasta Itens Recuperáveis. For more information, see the following topics:

- [Procurar e eliminar mensagens](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Caixa de correio de pesquisa](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

Para caixas de correio que estejam em espera, os administradores têm de remover o porão antes de poderem eliminar itens da pasta Itens Recuperáveis. Para obter mais informações, consulte [eliminar itens na pasta Itens Recuperáveis de caixas de correio baseadas na nuvem em espera](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

Para ajudar a evitar que a pasta de Itens Recuperáveis fique cheia, os administradores podem aumentar o limite de armazenamento da pasta Itens Recuperáveis para caixas de correio em espera e configurar uma política de retenção de caixas de correio que transfere os itens da pasta Itens Recuperáveis para a caixa de correio do utilizador. Ver [Aumentar a quota de itens recuperáveis para caixas de correio em espera](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
