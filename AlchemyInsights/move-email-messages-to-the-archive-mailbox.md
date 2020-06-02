---
title: Mova mensagens de e-mail para a caixa de correio do Arquivo
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 35c11f1bfb7c61b28a64f0128c29ddf7b4fce939
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511051"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="1ce5c-102">Mova o e-mail para a caixa de correio do arquivo</span><span class="sxs-lookup"><span data-stu-id="1ce5c-102">Move email to the archive mailbox</span></span>

1. <span data-ttu-id="1ce5c-103">Confirme se foi ativada uma **caixa de correio archive.**</span><span class="sxs-lookup"><span data-stu-id="1ce5c-103">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="1ce5c-104">Caso contrário, utilize os passos [deste artigo](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) para ativar a caixa de correio de arquivo.</span><span class="sxs-lookup"><span data-stu-id="1ce5c-104">If not, use the steps in [this article](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="1ce5c-105">Para arquivar automaticamente as mensagens na caixa de correio de arquivo, deve ser definida uma etiqueta de retenção com a ação **Move to archive** para ser aplicada automaticamente na **marcação completa da caixa de correio (predefinição).**</span><span class="sxs-lookup"><span data-stu-id="1ce5c-105">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="1ce5c-106">Utilize os passos aqui para criar a etiqueta: [Etiqueta Padrão de Arquivo](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="1ce5c-106">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="1ce5c-107">Em seguida, adicione a etiqueta **Archive** à sua política de retenção.</span><span class="sxs-lookup"><span data-stu-id="1ce5c-107">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="1ce5c-108">No centro de administração Exchange, escolha **Políticas de Retenção** > adicione a **etiqueta Move to Archive** à política > **Salvar**.</span><span class="sxs-lookup"><span data-stu-id="1ce5c-108">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="1ce5c-109">Agora [atribua a Política de Retenção](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) à caixa de correio específica do utilizador.</span><span class="sxs-lookup"><span data-stu-id="1ce5c-109">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="1ce5c-110">A mesma política será aplicada tanto à **caixa de** correio Primária como ao **Arquivo.**</span><span class="sxs-lookup"><span data-stu-id="1ce5c-110">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="1ce5c-111">Pode ser necessário forçar o Assistente de Pasta Gerida (MFA) a executar e aplicar as novas definições na caixa de correio do utilizador.</span><span class="sxs-lookup"><span data-stu-id="1ce5c-111">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="1ce5c-112">Executar o seguinte comando enquanto [está ligado ao EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) para iniciar o Assistente de Pasta Gerida para uma caixa de correio específica:</span><span class="sxs-lookup"><span data-stu-id="1ce5c-112">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="1ce5c-113">Start-ManagedFolderAssistant -Identidade<name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="1ce5c-113">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="1ce5c-114">Para obter mais informações sobre a criação de uma política de arquivo, consulte [configurar uma política de arquivo e eliminação para caixas de correio](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="1ce5c-114">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  