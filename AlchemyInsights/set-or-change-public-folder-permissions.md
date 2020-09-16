---
title: Desembre ou altere permissões de pastas públicas
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
ms.assetid: cffdf9bf-34ce-40f6-a69e-d02f17d9caef
ms.openlocfilehash: c035d56ffade45cc4360a1d0dfca4c63bf110a38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771183"
---
# <a name="permissions-and-public-folders"></a>Permissões e Pastas Públicas

Pode alterar as permissões nas suas Pastas Públicas utilizando o Outlook, o Centro de Administração Exchange (EAC) ou PowerShell:
  
- Para obter instruções do Outlook, [clique aqui](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).
    
- Para a EAC, consulte [este artigo](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) para obter instruções. 
    
- Para Powershell, consulte [este artigo](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) para obter instruções sobre a utilização do comando Add-PublicFolderClientPermission. Se precisar de instruções para ligar ao Exchange Powershell, clique [aqui](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).
    
Se **os utilizadores externos não puderem enviar e-mails para uma Pasta Pública ativada por correio,** a razão pode ser que a pasta pública esteja a perder permissões necessárias para a entrega de emails externos. Pode corrigir isto utilizando as instruções do Outlook [aqui,](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1)ou as instruções PowerShell [aqui](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).
  

