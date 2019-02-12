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
ms.custom: Adm_O365
ms.assetid: cffdf9bf-34ce-40f6-a69e-d02f17d9caef
ms.openlocfilehash: e4e98ba3e7dff2bd86be4667d7262c9544f9c9cb
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/12/2019
ms.locfileid: "29899219"
---
# <a name="permissions-and-public-folders"></a>Permissões e as pastas públicas

Pode alterar as permissões em pastas públicas utilizando o Outlook, o Centro de administração do Exchange (EAC), ou o PowerShell:
  
- Para instruções do Outlook, [clique aqui](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).
    
- Para o EAC, consulte [Este artigo](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) para obter instruções. Pode clicar [aqui](https://support.office.com/article/ https://outlook.office365.com/ecp/.aspx) para navegar para EAC. 
    
- Para o Powershell, consulte [Este artigo](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) para obter instruções sobre como utilizar o commandlet adicionar PublicFolderClientPermission. Se necessitar de instruções para ligar ao Exchange Powershell, clique [aqui](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).
    
Se **utilizadores externos não é possível enviar mensagens de correio electrónico para uma pasta pública com correio electrónico**, o motivo poderá ser que a pasta pública não tem permissões necessárias para a entrega de correio electrónico externo. Pode corrigir esta situação utilizando as instruções do Outlook [aqui](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1), ou as instruções do PowerShell [aqui](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).
  

