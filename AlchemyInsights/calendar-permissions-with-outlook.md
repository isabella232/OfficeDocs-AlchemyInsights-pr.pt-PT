---
title: Permissões de Calendário
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: 78f27014c60badc801212177dd455ef2a0de5a9e
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862171"
---
# <a name="calendar-permissions"></a>Permissões de Calendário

Os utilizadores podem alterar as suas próprias Permissões de Calendário com o Outlook na Web ou outros clientes, mas como administrador poderá também ter de investigar.  
Com o Cmdlet Exchange PowerShell mostrar-lhe-á a permissão no calendário de um utilizador:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Para ver mais informações consulte o seguinte:

- [Get-MailboxPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

As permissões de calendário são usadas na partilha de calendários, para ver mais informações sobre a partilha de um calendário do Outlook, consulte estes artigos:

- [Partilhar um calendário do Outlook com outras pessoas](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Partilhe o seu calendário no Outlook na web para negócios](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Para resolver problemas, a Autorização do Calendário pode utilizar a ferramenta [Assistente de Assistência e Recuperação.](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f)