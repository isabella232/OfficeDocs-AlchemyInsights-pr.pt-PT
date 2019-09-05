---
title: Activar a auditoria de caixa de correio
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 73517f46935a67a4a8a3e4770090ac897fe67979
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/04/2019
ms.locfileid: "36736264"
---
# <a name="enable-mailbox-auditing"></a>Activar a auditoria de caixa de correio

Para activar a auditoria de caixa de correio para um único utilizador ou toda uma organização tem de ser executados de Shell Remota do energia os cmdlets seguintes:
  
 **Utilizador único**
  
Set-Mailbox - identidade "Joana Dow" - AuditEnabled $true
  
 **Organização**
  
Get-Mailbox - ResultSize ilimitado - filtrar {RecipientTypeDetails - eq "UserMailbox"} | Set-Mailbox - AuditEnabled $true
  
[Obter mais informações](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

