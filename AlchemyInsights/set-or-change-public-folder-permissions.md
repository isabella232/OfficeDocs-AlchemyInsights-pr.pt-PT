---
title: Definir ou alterar permissões de pasta pública
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 8/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: cffdf9bf-34ce-40f6-a69e-d02f17d9caef
ms.openlocfilehash: 8e6a51bcc47eac7e76f55700091ecd86bc1634d7
ms.sourcegitcommit: 5dee2fcb492bd922092a6de8045a95febe57b97e
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/06/2019
ms.locfileid: "29759831"
---
# <a name="permissions-and-public-folders"></a><span data-ttu-id="88883-102">Permissões e as pastas públicas</span><span class="sxs-lookup"><span data-stu-id="88883-102">Permissions and Public Folders</span></span>

<span data-ttu-id="88883-103">Pode alterar as permissões em pastas públicas utilizando o Outlook, o Centro de administração do Exchange (EAC), ou o PowerShell:</span><span class="sxs-lookup"><span data-stu-id="88883-103">You can change the permissions on your Public Folders using Outlook, the Exchange admin center (EAC), or PowerShell:</span></span>
  
- <span data-ttu-id="88883-104">Para instruções do Outlook, [clique aqui](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span><span class="sxs-lookup"><span data-stu-id="88883-104">For Outlook instructions, [click here](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span></span>
    
- <span data-ttu-id="88883-p101">Para o EAC, consulte [Este artigo](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) para obter instruções. Pode clicar [aqui](https://support.office.com/article/ https://outlook.office365.com/ecp/.aspx) para navegar para EAC.</span><span class="sxs-lookup"><span data-stu-id="88883-p101">For EAC, refer to [this article](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) for instructions. You can click [here](https://support.office.com/article/ https://outlook.office365.com/ecp/.aspx) to navigate to EAC.</span></span> 
    
- <span data-ttu-id="88883-p102">Para o Powershell, consulte [Este artigo](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) para obter instruções sobre como utilizar o commandlet adicionar PublicFolderClientPermission. Se necessitar de instruções para ligar ao Exchange Powershell, clique [aqui](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span><span class="sxs-lookup"><span data-stu-id="88883-p102">For Powershell, refer to [this article](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) for instructions on using the Add-PublicFolderClientPermission commandlet. If you need instructions to connect to Exchange Powershell, click [here](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span></span>
    
<span data-ttu-id="88883-p103">Se **utilizadores externos não é possível enviar mensagens de correio electrónico para uma pasta pública com correio electrónico**, o motivo poderá ser que a pasta pública não tem permissões necessárias para a entrega de correio electrónico externo. Pode corrigir esta situação utilizando as instruções do Outlook [aqui](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1), ou as instruções do PowerShell [aqui](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span><span class="sxs-lookup"><span data-stu-id="88883-p103">If **external users can't send emails to a mail-enabled Public Folder**, the reason might be that the public folder is missing permissions required for external email delivery. You can fix this using the Outlook instructions [here](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1), or the PowerShell instructions [here](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span></span>
  

