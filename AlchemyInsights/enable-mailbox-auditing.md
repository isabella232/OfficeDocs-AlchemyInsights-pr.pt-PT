---
title: Permitir a auditoria da caixa de correio
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 404ef9ecd824541f98471bb8797f5f6e025012b7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806302"
---
# <a name="enable-mailbox-auditing"></a>Permitir a auditoria da caixa de correio

Para ativar a auditoria da Caixa de Correio para um único utilizador ou para uma organização inteira, os seguintes cmdlets devem ser executados a partir de Remote Power Shell:
  
 **Utilizador Único**
  
Set-Mailbox -Identidade "Jane Dow" - AuditEnabled $true
  
 **Organização**
  
Get-Mailbox -ResultadoSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} Set-Mailbox -AuditEnabled $true
  
[Saiba mais](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing)
  

