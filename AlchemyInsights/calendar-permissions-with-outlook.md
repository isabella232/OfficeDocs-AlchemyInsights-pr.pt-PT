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
# <a name="calendar-permissions"></a><span data-ttu-id="9da12-102">Permissões de Calendário</span><span class="sxs-lookup"><span data-stu-id="9da12-102">Calendar Permissions</span></span>

<span data-ttu-id="9da12-103">Os utilizadores podem alterar as suas próprias Permissões de Calendário com o Outlook na Web ou outros clientes, mas como administrador poderá também ter de investigar.</span><span class="sxs-lookup"><span data-stu-id="9da12-103">Users can change their own Calendar Permissions with Outlook on the Web or other clients, but as an admin you may need to investigate as well.</span></span>  
<span data-ttu-id="9da12-104">Com o Cmdlet Exchange PowerShell mostrar-lhe-á a permissão no calendário de um utilizador:</span><span class="sxs-lookup"><span data-stu-id="9da12-104">With Exchange PowerShell cmdlet will show you the permission on a user’s calendar:</span></span>

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

<span data-ttu-id="9da12-105">Para ver mais informações consulte o seguinte:</span><span class="sxs-lookup"><span data-stu-id="9da12-105">To see more information see the following:</span></span>

- [<span data-ttu-id="9da12-106">Get-MailboxPermission</span><span class="sxs-lookup"><span data-stu-id="9da12-106">Get-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="9da12-107">Set-MailboxPermission</span><span class="sxs-lookup"><span data-stu-id="9da12-107">Set-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="9da12-108">Add-MailboxPermission</span><span class="sxs-lookup"><span data-stu-id="9da12-108">Add-MailboxFolderPermission</span></span>](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

<span data-ttu-id="9da12-109">As permissões de calendário são usadas na partilha de calendários, para ver mais informações sobre a partilha de um calendário do Outlook, consulte estes artigos:</span><span class="sxs-lookup"><span data-stu-id="9da12-109">Calendar Permissions are used in the sharing of calendars, to see more information about sharing an Outlook calendar, see these articles:</span></span>

- [<span data-ttu-id="9da12-110">Partilhar um calendário do Outlook com outras pessoas</span><span class="sxs-lookup"><span data-stu-id="9da12-110">Share an Outlook calendar with other people</span></span>](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [<span data-ttu-id="9da12-111">Partilhe o seu calendário no Outlook na web para negócios</span><span class="sxs-lookup"><span data-stu-id="9da12-111">Share your calendar in Outlook on the web for business</span></span>](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

<span data-ttu-id="9da12-112">Para resolver problemas, a Autorização do Calendário pode utilizar a ferramenta [Assistente de Assistência e Recuperação.](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f)</span><span class="sxs-lookup"><span data-stu-id="9da12-112">To troubleshoot Calendar Permission you can use the [Support and Recovery Assistant](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) tool.</span></span>