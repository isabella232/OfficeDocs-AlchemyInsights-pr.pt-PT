---
title: Políticas de retenção no Centro de administração do Exchange não funciona
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 73e8db432afccb73b872ec7a3ce84c25f1ba7f25
ms.sourcegitcommit: ca06ef831226d629de3057a0df85e017b80f3356
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/08/2019
ms.locfileid: "29786781"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Políticas de retenção no Centro de administração do Exchange

 **Problema:** Recentemente criados ou políticas de retenção actualizado no Centro de administração do Exchange não estão a aplicar às caixas de correio ou itens não são movidos para a caixa de correio do arquivo ou eliminadas. 
  
 **Causas raiz:**
  
- Isto pode ser porque o **Assistente da pasta gerida** não processou caixa de correio do utilizador. O Managed Assistente da pasta tenta processar cada caixa de correio na sua organização baseada na nuvem em sete dias. Se alterar um código de retenção ou aplicar uma política de retenção diferente a uma caixa de correio, pode esperar até que a pasta Assist geridos processa a caixa de correio ou pode executar o cmdlet Start-ManagedFolderAssistant para iniciar o Managed Assistente da pasta para processar um específico caixa de correio. Executar este cmdlet é útil para testar ou resolver problemas de definições de etiqueta de retenção ou de uma política de retenção. Para mais informações, visite a [executar o Managed Assistente da pasta](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Solução:** Execute o seguinte comando para iniciar o Managed Assistente da pasta para uma caixa de correio específica: 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Isto também pode ser ocorrer se **RetentionHold** tiver sido **activada** a caixa de correio. Se a caixa de correio tiver sido colocada sobre uma RetentionHold, a política de retenção sobre a caixa de correio não será processada durante esse período. Para mais informações sobre sobre consulte de definição RetentionHold: [Mantenha de retenção de caixa de correio](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Solução:**
    
  - Verifique o estado da definição da caixa de correio específica no [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)RetentionHold:
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Execute o seguinte comando para **desactivar a** RetentionHold numa caixa de correio específica: 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Agora, volte a executar a Assistente de pasta geridos:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Nota:** Se uma caixa de correio for inferior a 10 MB, o Managed Assistente da pasta não irá automaticamente processar a caixa de correio. 
  

