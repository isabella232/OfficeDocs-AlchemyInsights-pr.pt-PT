---
title: 1336 A pastaItens Recuperáveis está cheia
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
ms.openlocfilehash: 5c8d53ceabf2428f3d6d765040f1b789b6bbeda04a22dd7fde0d2d728fd17d93
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54061767"
---
# <a name="the-recoverable-items-folder-is-full"></a>A pasta Itens Recuperáveis está cheia

Para Exchange Online correio, o limite de armazenamento predefinido para a pasta Itens Recuperáveis é de 30 GB. O limite de armazenamento da pasta Itens Recuperáveis é automaticamente aumentado para 100 GB se a caixa de correio for colocada em Retenção de Litigação, na Deteção de Dados Eletrónicos ou se for atribuída a uma política de retenção.

Quando a pasta Itens Recuperáveis atinge o limite de armazenamento, a funcionalidade da caixa de correio é afetada das seguintes formas:

- O utilizador não pode eliminar itens da caixa de correio.

- O Assistente de Pastas Geridas não pode eliminar itens com base nas definições da etiqueta de retenção ou da pasta gerida.

- Para caixas de correio com a Recuperação de Itens Únicos ativada ou colocada em espera, o processo de proteção de página de escrita não consegue manter versões de itens editados pelo utilizador.

- Para caixas de correio com o registo de auditoria de caixa de correio ativado, não é possível guardá-los na subpasta Auditorias na pasta Itens Recuperáveis.

Para caixas de correio que não estão em espera, os administradores podem utilizar o comando no Exchange Online PowerShell para eliminar itens na pasta Itens `Search-Mailbox -SearchDumpsterOnly -DeleteContent` Recuperáveis. For more information, see the following topics:

- [Procurar e eliminar mensagens](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

Para as caixas de correio que estão em espera, os administradores têm de remover a remoção da mesma antes de poderem eliminar itens da pasta Itens Recuperáveis. Para obter mais informações, consulte Eliminar itens na pasta Itens Recuperáveis de caixas de correio [baseadas na nuvem em espera.](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold)

Para ajudar a impedir que a pasta Itens Recuperáveis esteja cheia, os administradores podem aumentar o limite de armazenamento da pasta Itens Recuperáveis para caixas de correio em espera e configurar uma política de retenção de caixas de correio que move itens da pasta Itens Recuperáveis para a caixa de correio de arquivo do utilizador. Consulte [Aumentar a quota de Itens Recuperáveis para caixas de correio em espera.](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold)
