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
ms.openlocfilehash: a631af20e28a531a40f078e290239a372c38ab74
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/12/2019
ms.locfileid: "29941725"
---
Problemas ao arquivo de itens na caixa de correio do arquivo. Certifique-se de que mandar efectuar os seguintes passos:
  
1. Confirme que a um **arquivo de caixa de correio** foi activada. Caso contrário, utilize os passos [neste](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) artigo para activar a caixa de correio do arquivo. 
    
2. No Centro de administração do Exchange, seleccione **Os códigos de retenção** em **Gestão de conformidade**, criar uma **tag de retenção** com a acção de **Mover para o arquivo** de mensagens em fila que contém a **Idade de retenção**de pretendido.
    
3. No Centro de administração do Exchange, seleccione **As políticas de retenção**, criar uma **Política de retenção** e adicione o código de retenção **Mover para arquivo** para essa política. 
    
4. [Atribuir a política de retenção](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) a caixa de correio do utilizador específico. A mesma política será aplicada para o **principal** e a caixa de correio do **arquivo** . 
    
Caixa de correio do utilizador deverá ter uma política de arquivo para mover itens para a caixa de correio do arquivo. Poderá ser necessário forçar o Managed pasta Assistente (AMF) para executar e aplicar as novas definições a caixa de correio do utilizador. Execute o seguinte comando enquanto [ligado à EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) para iniciar o Managed Assistente da pasta para uma caixa de correio específica: 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

Para mais informações sobre como configurar uma política de arquivo, consulte [Configurar uma política de arquivo e eliminação para caixas de correio](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  

