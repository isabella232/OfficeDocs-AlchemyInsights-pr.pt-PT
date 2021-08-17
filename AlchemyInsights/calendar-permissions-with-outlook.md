---
title: Permissões do Calendário
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
- "3800009"
- "611"
ms.openlocfilehash: 4bf7680a422f096401f0a87bccd1b8dd11f4489f882bcc06864e37d6a248438c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046115"
---
# <a name="calendar-permissions"></a>Permissões do Calendário

Os utilizadores podem alterar as suas próprias Permissões de Calendário Outlook com o Outlook na Web ou outros clientes, mas enquanto administrador também poderá ter de investigar.  
Com Exchange cmdlet do PowerShell irá mostrar-lhe a permissão num calendário de utilizador:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Para ver mais informações, consulte o seguinte:

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

As Permissões de Calendário são utilizadas na partilha de calendários. Para ver mais informações sobre como partilhar um calendário Outlook, consulte estes artigos:

- [Partilhar um calendário do Outlook com outras pessoas](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Partilhar o seu calendário no Outlook na Web para empresas](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Para remoção de Permissões de Calendário, pode utilizar [a Assistente de Recuperação e Suporte](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) Calendário.