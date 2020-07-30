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
ms.openlocfilehash: 4d3ca121c8d22a0900f136f7f2a754dfb5b435f5
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/29/2020
ms.locfileid: "46522818"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="82e23-102">Políticas de Retenção no Centro de Administração de Intercâmbio</span><span class="sxs-lookup"><span data-stu-id="82e23-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="82e23-103">Se quiser que façamos verificações automatizadas das definições abaixo mencionadas, selecione o botão de trás <-- no topo desta página e, em seguida, insira o endereço de e-mail do utilizador que tem problemas com as políticas de retenção.</span><span class="sxs-lookup"><span data-stu-id="82e23-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

 <span data-ttu-id="82e23-104">**Emissão:** As políticas de retenção recentemente criadas ou atualizadas no Exchange Admin Center não estão a ser aplicadas a caixas de correio ou os itens não são transferidos para a caixa de correio de arquivo ou eliminados.</span><span class="sxs-lookup"><span data-stu-id="82e23-104">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="82e23-105">**Causas de raiz:**</span><span class="sxs-lookup"><span data-stu-id="82e23-105">**Root Causes:**</span></span>
  
- <span data-ttu-id="82e23-106">Isto pode ser porque o **Assistente de Pasta Gerida** não processou a caixa de correio do utilizador.</span><span class="sxs-lookup"><span data-stu-id="82e23-106">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="82e23-107">O Assistente de Pasta Gerida tenta processar todas as caixas de correio da sua organização baseada na nuvem uma vez a cada sete dias.</span><span class="sxs-lookup"><span data-stu-id="82e23-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="82e23-108">Se alterar uma etiqueta de retenção ou aplicar uma política de retenção diferente a uma caixa de correio, pode esperar até que o Serviço de Assistência à Pasta Gerida processe a caixa de correio, ou pode executar a cmdlet Start-ManagedFolderAssistant para iniciar o Assistente de Pasta Gerida para processar uma caixa de correio específica.</span><span class="sxs-lookup"><span data-stu-id="82e23-108">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="82e23-109">A execução deste cmdlet é útil para testar ou resolver problemas de uma política de retenção ou configurações de etiquetas de retenção.</span><span class="sxs-lookup"><span data-stu-id="82e23-109">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="82e23-110">Para mais informações, visite [executar o Assistente de Pasta Gerida](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="82e23-110">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="82e23-111">**Solução:** Executar o seguinte comando para iniciar o Assistente de Pasta Gerida para uma caixa de correio específica:</span><span class="sxs-lookup"><span data-stu-id="82e23-111">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="82e23-112">Isto também pode ocorrer se **o RetentionHold** tiver sido **ativado** na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="82e23-112">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="82e23-113">Se a caixa de correio tiver sido colocada num RetentionHold, a política de retenção na caixa de correio não será processada durante esse período.</span><span class="sxs-lookup"><span data-stu-id="82e23-113">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="82e23-114">Para obter mais informação sobre a definição Retençãoremente ver: [Retenção de caixa de correio .](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)</span><span class="sxs-lookup"><span data-stu-id="82e23-114">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="82e23-115">**Solução:**</span><span class="sxs-lookup"><span data-stu-id="82e23-115">**Solution:**</span></span>
    
  - <span data-ttu-id="82e23-116">Verifique o estado da definição RetentionHold na caixa de correio específica em [exo powershell:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="82e23-116">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="82e23-117">Executar o seguinte comando para **desativar** o RetentionHold numa caixa de correio específica:</span><span class="sxs-lookup"><span data-stu-id="82e23-117">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="82e23-118">Agora, reencamina o Assistente de Pasta Gerida:</span><span class="sxs-lookup"><span data-stu-id="82e23-118">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="82e23-119">**Nota:** Se uma caixa de correio for inferior a 10 MB, o Assistente de Pasta Gerida não processará automaticamente a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="82e23-119">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="82e23-120">Para obter mais informações sobre as políticas de retenção no Exchange Admin Center, consulte:</span><span class="sxs-lookup"><span data-stu-id="82e23-120">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="82e23-121">Etiquetas de retenção e políticas de retenção</span><span class="sxs-lookup"><span data-stu-id="82e23-121">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="82e23-122">Aplicar uma política de retenção nas caixas de correio</span><span class="sxs-lookup"><span data-stu-id="82e23-122">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="82e23-123">Adicione ou remova etiquetas de retenção</span><span class="sxs-lookup"><span data-stu-id="82e23-123">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="82e23-124">Como identificar o tipo de porão colocado numa caixa de correio</span><span class="sxs-lookup"><span data-stu-id="82e23-124">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
