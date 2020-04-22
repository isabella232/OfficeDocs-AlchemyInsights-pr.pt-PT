---
title: Mover mensagens de correio eletrónico para a caixa de correio do Arquivo
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
ms.openlocfilehash: a5ad81e97df0ed5c337a622126173df94af80bb8
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713657"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="7f9ca-102">Mova o e-mail para a caixa de correio de arquivo</span><span class="sxs-lookup"><span data-stu-id="7f9ca-102">Move email to the archive mailbox</span></span>

1. <span data-ttu-id="7f9ca-103">Confirme que foi ativada uma **caixa de correio Archive.**</span><span class="sxs-lookup"><span data-stu-id="7f9ca-103">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="7f9ca-104">Caso contrário, utilize os passos [deste artigo](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) para ativar a caixa de correio de arquivo.</span><span class="sxs-lookup"><span data-stu-id="7f9ca-104">If not, use the steps in [this article](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="7f9ca-105">Para arquivar mensagens automaticamente na caixa de correio de arquivo, deve ser definida uma etiqueta de retenção com o **Movimento para arquivar** ação para ser aplicada automaticamente à etiqueta inteira da caixa de correio **(predefinido).**</span><span class="sxs-lookup"><span data-stu-id="7f9ca-105">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="7f9ca-106">Utilize os passos aqui para criar a etiqueta: [Etiqueta padrão de arquivo](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="7f9ca-106">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="7f9ca-107">Em seguida, adicione a etiqueta **de Arquivo** à sua política de retenção.</span><span class="sxs-lookup"><span data-stu-id="7f9ca-107">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="7f9ca-108">No centro de administração exchange, escolha Políticas de **Retenção** > adicione a **etiqueta Move to Archive** à política > **Save**.</span><span class="sxs-lookup"><span data-stu-id="7f9ca-108">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="7f9ca-109">Agora [atribua a Política](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) de Retenção à caixa de correio do utilizador específico.</span><span class="sxs-lookup"><span data-stu-id="7f9ca-109">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="7f9ca-110">A mesma política será aplicada tanto à **Primary** como à **Caixa** de Correio seleções.</span><span class="sxs-lookup"><span data-stu-id="7f9ca-110">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="7f9ca-111">Pode ser necessário forçar o Assistente de Pasta Gerida (MFA) a executar e aplicar as novas definições na caixa de correio do utilizador.</span><span class="sxs-lookup"><span data-stu-id="7f9ca-111">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="7f9ca-112">Executar o seguinte comando enquanto [ligado ao EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) para iniciar o Assistente de Pasta Gerida para uma caixa de correio específica:</span><span class="sxs-lookup"><span data-stu-id="7f9ca-112">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="7f9ca-113">Assistente de Pasta Gerido por Início -Identidade<name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="7f9ca-113">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="7f9ca-114">Para obter mais informações sobre a criação de uma política de arquivo, consulte [A criação de uma política de arquivo e eliminação para caixas de correio](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="7f9ca-114">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  