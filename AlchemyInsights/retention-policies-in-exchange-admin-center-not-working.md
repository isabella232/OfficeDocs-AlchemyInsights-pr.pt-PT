---
title: Políticas de Retenção no Exchange Admin Center não funcionam
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: e2fb22f872be0eefc3b4b78b18cd09baffa66cda
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742444"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Políticas de Retenção no Centro de Administração de Intercâmbio

 **Emissão:** As políticas de retenção recentemente criadas ou atualizadas no Exchange Admin Center não se aplicam a caixas de correio ou itens não são transferidos para a caixa de correio de arquivo ou eliminados. 
  
 **Causas de raiz:**
  
- Isto pode acontecer porque o Assistente de **Pasta Gerida** não processou a caixa de correio do utilizador. O Assistente de Pasta Gerida tenta processar todas as caixas de correio da sua organização baseada na nuvem uma vez a cada sete dias. Se alterar uma etiqueta de retenção ou aplicar uma política de retenção diferente numa caixa de correio, pode esperar até que o Serviço de Assistência à Pasta Gerida processe a caixa de correio, ou pode executar o cmdlet Start-ManagedFolderAssistant para iniciar o Assistente de Pasta Gerida para processar uma caixa de correio específica. Executar este cmdlet é útil para testar ou resolver problemas uma política de retenção ou definições de etiquetade retenção. Para mais informações, visite [Executar o Assistente](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist)de Pasta Gerida .
    
  - **Solução:** Executar o seguinte comando para iniciar o Assistente de Pasta Gerida para uma caixa de correio específica:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Isto também pode ocorrer se **o RetentionHold** tiver sido **ativado** na caixa de correio. Se a caixa de correio tiver sido colocada num RetentionHold, a política de retenção na caixa de correio não será processada durante esse período. Para mais informações sobre a definição RetentionHold ver: [Retenção](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)de caixas de correio .
    
    **Solução:**
    
  - Verifique o estado da definição retentionHold na caixa de correio específica em [exo powershell:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Executar o seguinte comando para **desativar** RetentionHold numa caixa de correio específica:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Agora, reexecutar a pasta Gerida Assistente:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Nota:** Se uma caixa de correio for inferior a 10 MB, o Assistente de Pasta Gerida não processará automaticamente a caixa de correio.
 
Para obter mais informações sobre as políticas de retenção no Exchange Admin Center, consulte:
- [Etiquetas de retenção e políticas de retenção](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Aplicar uma política de retenção nas caixas de correio](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Adicionar ou remover etiquetas de retenção](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Como identificar o tipo de porão colocado numa caixa de correio](https://docs.microsoft.com/office365/securitycompliance/identify-a-hold-on-an-exchange-online-mailbox)
