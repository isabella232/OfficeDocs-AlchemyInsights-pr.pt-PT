---
title: Definir ou alterar permissões de pasta pública
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 8/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cffdf9bf-34ce-40f6-a69e-d02f17d9caef
ms.openlocfilehash: 1015c2203406e15d6b418c387b6632a182d6d2ff
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/04/2019
ms.locfileid: "36734680"
---
# <a name="permissions-and-public-folders"></a>Permissões e as pastas públicas

Pode alterar as permissões em pastas públicas utilizando o Outlook, o Centro de administração do Exchange (EAC), ou o PowerShell:
  
- Para instruções do Outlook, [clique aqui](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).
    
- Para o EAC, consulte [Este artigo](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) para obter instruções. 
    
- Para o Powershell, consulte [Este artigo](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) para obter instruções sobre como utilizar o commandlet adicionar PublicFolderClientPermission. Se necessitar de instruções para ligar ao Exchange Powershell, clique [aqui](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).
    
Se **utilizadores externos não é possível enviar mensagens de correio electrónico para uma pasta pública com correio electrónico**, o motivo poderá ser que a pasta pública não tem permissões necessárias para a entrega de correio electrónico externo. Pode corrigir esta situação utilizando as instruções do Outlook [aqui](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1), ou as instruções do PowerShell [aqui](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).
  

