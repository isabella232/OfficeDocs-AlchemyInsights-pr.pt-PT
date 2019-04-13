---
title: 1336 RecoverableItems pasta está cheia
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1336
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 14d46980caf7dac90e73c34482a3aee34382fa1f
ms.sourcegitcommit: 1a4b8fa9e38a95ca811085af516edb81caf2018c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/13/2019
ms.locfileid: "31859007"
---
# <a name="the-recoverable-items-folder-is-full"></a>A pasta de itens recuperável está cheia

Para caixas de correio Exchange Online no Office 365, o limite de armazenamento predefinida para a pasta itens recuperável é 30 GB. O limite de armazenamento para a pasta de itens recuperável automaticamente é aumentado para 100 GB se a caixa de correio é colocada em suspensão do litígio, suspenso de detecção de dados electrónicos, ou atribuída a uma política de retenção do Office 365.

Quando a pasta itens recuperável atinge o limite de armazenamento, a funcionalidade de caixa de correio é afectada das seguintes formas:

- O utilizador não é possível eliminar itens da caixa de correio.

- O Managed Assistente da pasta não pode eliminar itens com base no código de retenção ou as definições de pasta gerida.

- Para caixas de correio que tenham o único Item recuperação activada ou colocadas em espera, o processo de protecção de página de cópia de escrita não é possível manter versões dos itens editados pelo utilizador.

- Para caixas de correio que tenham activado o registo de auditoria da caixa de correio, entradas de registo de auditoria sem caixa de correio podem ser guardadas na subpasta auditorias na pasta itens recuperável.

Para caixas de correio que não estão em espera, admins pode utilizar o `Search-Mailbox -SearchDumpsterOnly -DeleteContent` comando no PowerShell Online do Exchange para eliminar itens na pasta itens recuperável. For more information, see the following topics: 

- [Procurar e eliminar mensagens](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)

- [Caixa de correio de procura](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

Para caixas de correio que estão em espera, admins devem remover o antes de poderem itens eliminados da pasta itens recuperável. Para mais informações, consulte [Eliminar itens em itens recuperável mantenha pasta baseada na nuvem caixas de correio](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

Para ajudar a evitar que a pasta itens recuperável se torne completo, admins pode aumentar o limite de armazenamento dos itens recuperável mantenha a tecla de pasta para caixas de correio e configurar uma política de retenção de caixa de correio que move itens da pasta itens recuperável para arquivo do utilizador caixa de correio. Consulte a [aumentar os itens recuperável mantenha de quota para caixas de correio](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
