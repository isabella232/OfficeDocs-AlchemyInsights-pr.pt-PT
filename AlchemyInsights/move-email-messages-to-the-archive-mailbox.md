---
title: Mover mensagens de correio electrónico na caixa de correio do arquivo
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 37f256ef31402f5139fdd7c2af8f3a6ca9dc3525
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32418336"
---
# <a name="move-email-to-the-archive-mailbox"></a>Mover a mensagem de correio electrónico na caixa de correio do arquivo
 
1. Confirme que a um **arquivo de caixa de correio** foi activada. Caso contrário, utilize os passos [neste](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) artigo para activar a caixa de correio do arquivo.

2. Para arquivar mensagens automaticamente para a caixa de correio do arquivo, tem de ser definido um código de retenção com a acção de **Mover para arquivar** aplicado **automaticamente a tag de caixa de correio inteiro (predefinição)**. Utilize os passos aqui para criar a tag: [tag de arquivo predefinido](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0).
    
3. Em seguida, adicione a tag de **arquivo** para a política de retenção. No Centro de administração de Exchange, escolha **As políticas de retenção** > adicionar **mover a tag de arquivo** para o > de política **Guardar**. 
    
4. Agora a [atribuir a política de retenção](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) a caixa de correio do utilizador específico. A mesma política será aplicada para o **principal** e a caixa de correio do **arquivo** . 
    
Poderá ser necessário forçar o Managed pasta Assistente (AMF) para executar e aplicar as novas definições a caixa de correio do utilizador. Execute o seguinte comando enquanto [ligado à EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) para iniciar o Managed Assistente da pasta para uma caixa de correio específica: 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

Para mais informações sobre como configurar uma política de arquivo, consulte [Configurar uma política de arquivo e eliminação para caixas de correio](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  

