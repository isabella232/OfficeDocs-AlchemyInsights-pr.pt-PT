---
title: Políticas de Retenção no Centro de Administração de Intercâmbio não funcionam
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
ms.openlocfilehash: 3040365b9d686bcbcce60977ee9bdbbaffc70b24
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44502618"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="0b362-102">Políticas de Retenção no Centro de Administração de Intercâmbio</span><span class="sxs-lookup"><span data-stu-id="0b362-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="0b362-103">**Emissão:** As políticas de retenção recentemente criadas ou atualizadas no Exchange Admin Center não estão a ser aplicadas a caixas de correio ou os itens não são transferidos para a caixa de correio de arquivo ou eliminados.</span><span class="sxs-lookup"><span data-stu-id="0b362-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="0b362-104">**Causas de raiz:**</span><span class="sxs-lookup"><span data-stu-id="0b362-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="0b362-105">Isto pode ser porque o **Assistente de Pasta Gerida** não processou a caixa de correio do utilizador.</span><span class="sxs-lookup"><span data-stu-id="0b362-105">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="0b362-106">O Assistente de Pasta Gerida tenta processar todas as caixas de correio da sua organização baseada na nuvem uma vez a cada sete dias.</span><span class="sxs-lookup"><span data-stu-id="0b362-106">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="0b362-107">Se alterar uma etiqueta de retenção ou aplicar uma política de retenção diferente a uma caixa de correio, pode esperar até que o Serviço de Assistência à Pasta Gerida processe a caixa de correio, ou pode executar a cmdlet Start-ManagedFolderAssistant para iniciar o Assistente de Pasta Gerida para processar uma caixa de correio específica.</span><span class="sxs-lookup"><span data-stu-id="0b362-107">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="0b362-108">A execução deste cmdlet é útil para testar ou resolver problemas de uma política de retenção ou configurações de etiquetas de retenção.</span><span class="sxs-lookup"><span data-stu-id="0b362-108">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="0b362-109">Para mais informações, visite [executar o Assistente de Pasta Gerida](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="0b362-109">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="0b362-110">**Solução:** Executar o seguinte comando para iniciar o Assistente de Pasta Gerida para uma caixa de correio específica:</span><span class="sxs-lookup"><span data-stu-id="0b362-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="0b362-111">Isto também pode ocorrer se **o RetentionHold** tiver sido **ativado** na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="0b362-111">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="0b362-112">Se a caixa de correio tiver sido colocada num RetentionHold, a política de retenção na caixa de correio não será processada durante esse período.</span><span class="sxs-lookup"><span data-stu-id="0b362-112">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="0b362-113">Para obter mais informação sobre a definição Retençãoremente ver: [Retenção de caixa de correio .](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)</span><span class="sxs-lookup"><span data-stu-id="0b362-113">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="0b362-114">**Solução:**</span><span class="sxs-lookup"><span data-stu-id="0b362-114">**Solution:**</span></span>
    
  - <span data-ttu-id="0b362-115">Verifique o estado da definição RetentionHold na caixa de correio específica em [exo powershell:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="0b362-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="0b362-116">Executar o seguinte comando para **desativar** o RetentionHold numa caixa de correio específica:</span><span class="sxs-lookup"><span data-stu-id="0b362-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="0b362-117">Agora, reencamina o Assistente de Pasta Gerida:</span><span class="sxs-lookup"><span data-stu-id="0b362-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="0b362-118">**Nota:** Se uma caixa de correio for inferior a 10 MB, o Assistente de Pasta Gerida não processará automaticamente a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="0b362-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="0b362-119">Para obter mais informações sobre as políticas de retenção no Exchange Admin Center, consulte:</span><span class="sxs-lookup"><span data-stu-id="0b362-119">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="0b362-120">Etiquetas de retenção e políticas de retenção</span><span class="sxs-lookup"><span data-stu-id="0b362-120">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="0b362-121">Aplicar uma política de retenção nas caixas de correio</span><span class="sxs-lookup"><span data-stu-id="0b362-121">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="0b362-122">Adicione ou remova etiquetas de retenção</span><span class="sxs-lookup"><span data-stu-id="0b362-122">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="0b362-123">Como identificar o tipo de porão colocado numa caixa de correio</span><span class="sxs-lookup"><span data-stu-id="0b362-123">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
