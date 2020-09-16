---
title: Políticas de Retenção no Centro de Administração de Intercâmbio não funcionam
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 1fee2361b2dd6e0989d430a17aebb13bd5948578
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740521"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Políticas de Retenção no Centro de Administração de Intercâmbio

Se quiser que façamos verificações automatizadas das definições abaixo mencionadas, selecione o botão de trás <-- no topo desta página e, em seguida, insira o endereço de e-mail do utilizador que tem problemas com as políticas de retenção.

 **Emissão:** As políticas de retenção recentemente criadas ou atualizadas no Exchange Admin Center não estão a ser aplicadas a caixas de correio ou os itens não são transferidos para a caixa de correio de arquivo ou eliminados. 
  
 **Causas de raiz:**
  
- Isto pode ser porque o **Assistente de Pasta Gerida** não processou a caixa de correio do utilizador. O Assistente de Pasta Gerida tenta processar todas as caixas de correio da sua organização baseada na nuvem uma vez a cada sete dias. Se alterar uma etiqueta de retenção ou aplicar uma política de retenção diferente a uma caixa de correio, pode esperar até que o Serviço de Assistência à Pasta Gerida processe a caixa de correio, ou pode executar a cmdlet Start-ManagedFolderAssistant para iniciar o Assistente de Pasta Gerida para processar uma caixa de correio específica. A execução deste cmdlet é útil para testar ou resolver problemas de uma política de retenção ou configurações de etiquetas de retenção. Para mais informações, visite [executar o Assistente de Pasta Gerida](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Solução:** Executar o seguinte comando para iniciar o Assistente de Pasta Gerida para uma caixa de correio específica:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Isto também pode ocorrer se **o RetentionHold** tiver sido **ativado** na caixa de correio. Se a caixa de correio tiver sido colocada num RetentionHold, a política de retenção na caixa de correio não será processada durante esse período. Para obter mais informação sobre a definição Retençãoremente ver: [Retenção de caixa de correio .](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)
    
    **Solução:**
    
  - Verifique o estado da definição RetentionHold na caixa de correio específica em [exo powershell:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Executar o seguinte comando para **desativar** o RetentionHold numa caixa de correio específica:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Agora, reencamina o Assistente de Pasta Gerida:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Nota:** Se uma caixa de correio for inferior a 10 MB, o Assistente de Pasta Gerida não processará automaticamente a caixa de correio.
 
Para obter mais informações sobre as políticas de retenção no Exchange Admin Center, consulte:
- [Etiquetas de retenção e políticas de retenção](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Aplicar uma política de retenção nas caixas de correio](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Adicione ou remova etiquetas de retenção](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Como identificar o tipo de porão colocado numa caixa de correio](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
