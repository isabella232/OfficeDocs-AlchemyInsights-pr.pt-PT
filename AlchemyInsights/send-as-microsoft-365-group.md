---
title: Enviar Como Microsoft grupo 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/19/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: cfb4bd5ce59eeccdd0812d013b8a444aebeb1d4c
ms.sourcegitcommit: 9818d3c8e6b10f23244e51286e2463caf48fffd5
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/21/2020
ms.locfileid: "46872060"
---
# <a name="send-as-microsoft-365-group"></a>Enviar Como Microsoft grupo 365

Pode atribuir permissões de Envio como para permitir que utilizadores específicos enviem mensagens como um grupo Microsoft 365:  

1. Ligue-se a Exchange Online PowerShell.  

2. Run the following command:  

    Add-RecipientPermission `<GroupName>` -Trustee `<MailboxName>` -AccessRights SendAs

Para obter mais informações, consulte [Permitir que os membros enviem como ou enviem em nome de um grupo](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide).