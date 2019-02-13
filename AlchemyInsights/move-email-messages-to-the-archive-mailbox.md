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
<span data-ttu-id="45f04-p101">Problemas ao arquivo de itens na caixa de correio do arquivo. Certifique-se de que mandar efectuar os seguintes passos:</span><span class="sxs-lookup"><span data-stu-id="45f04-p101">Having problems archiving items to the Archive mailbox. Make sure you have performed the following steps:</span></span>
  
1. <span data-ttu-id="45f04-p102">Confirme que a um **arquivo de caixa de correio** foi activada. Caso contrário, utilize os passos [neste](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) artigo para activar a caixa de correio do arquivo.</span><span class="sxs-lookup"><span data-stu-id="45f04-p102">Confirm that an **Archive mailbox** has been enabled. If not, use steps in [this article](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span> 
    
2. <span data-ttu-id="45f04-106">No Centro de administração do Exchange, seleccione **Os códigos de retenção** em **Gestão de conformidade**, criar uma **tag de retenção** com a acção de **Mover para o arquivo** de mensagens em fila que contém a **Idade de retenção**de pretendido.</span><span class="sxs-lookup"><span data-stu-id="45f04-106">In the Exchange Admin Center, select **Retention Tags** under **Compliance Management**, create a **Retention tag** with the **Move to Archive** action containing the desired **Retention Age**.</span></span>
    
3. <span data-ttu-id="45f04-107">No Centro de administração do Exchange, seleccione **As políticas de retenção**, criar uma **Política de retenção** e adicione o código de retenção **Mover para arquivo** para essa política.</span><span class="sxs-lookup"><span data-stu-id="45f04-107">In the Exchange Admin Center, select **Retention Policies**, create a **Retention Policy** and add your **Move to Archive** retention tag to that policy.</span></span> 
    
4. <span data-ttu-id="45f04-p103">[Atribuir a política de retenção](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) a caixa de correio do utilizador específico. A mesma política será aplicada para o **principal** e a caixa de correio do **arquivo** .</span><span class="sxs-lookup"><span data-stu-id="45f04-p103">[Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox. The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span> 
    
<span data-ttu-id="45f04-p104">Caixa de correio do utilizador deverá ter uma política de arquivo para mover itens para a caixa de correio do arquivo. Poderá ser necessário forçar o Managed pasta Assistente (AMF) para executar e aplicar as novas definições a caixa de correio do utilizador. Execute o seguinte comando enquanto [ligado à EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) para iniciar o Managed Assistente da pasta para uma caixa de correio específica:</span><span class="sxs-lookup"><span data-stu-id="45f04-p104">The user's mailbox should now have an Archive policy to move items to the Archive mailbox. It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox. Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span> 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

<span data-ttu-id="45f04-113">Para mais informações sobre como configurar uma política de arquivo, consulte [Configurar uma política de arquivo e eliminação para caixas de correio](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="45f04-113">Want more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  

