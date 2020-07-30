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
ms.openlocfilehash: 9af8a4d3ce72fd901ff2f3a1aae0654c7213dd7e
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/29/2020
ms.locfileid: "46522782"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="32554-102">Mova o e-mail para a caixa de correio do arquivo</span><span class="sxs-lookup"><span data-stu-id="32554-102">Move email to the archive mailbox</span></span>

<span data-ttu-id="32554-103">Se quiser que façamos verificações automatizadas das definições abaixo mencionadas, selecione o botão de trás <-- no topo desta página e, em seguida, insira o endereço de e-mail do utilizador que tem problemas em transferir o e-mail para a sua caixa de correio de arquivo.</span><span class="sxs-lookup"><span data-stu-id="32554-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems moving email to their archive mailbox.</span></span>

1. <span data-ttu-id="32554-104">Confirme se foi ativada uma **caixa de correio archive.**</span><span class="sxs-lookup"><span data-stu-id="32554-104">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="32554-105">Caso contrário, utilize os passos [deste artigo](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) para ativar a caixa de correio de arquivo.</span><span class="sxs-lookup"><span data-stu-id="32554-105">If not, use the steps in [this article](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="32554-106">Para arquivar automaticamente as mensagens na caixa de correio de arquivo, deve ser definida uma etiqueta de retenção com a ação **Move to archive** para ser aplicada automaticamente na **marcação completa da caixa de correio (predefinição).**</span><span class="sxs-lookup"><span data-stu-id="32554-106">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="32554-107">Utilize os passos aqui para criar a etiqueta: [Etiqueta Padrão de Arquivo](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="32554-107">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="32554-108">Em seguida, adicione a etiqueta **Archive** à sua política de retenção.</span><span class="sxs-lookup"><span data-stu-id="32554-108">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="32554-109">No centro de administração Exchange, escolha **Políticas de Retenção** > adicione a **etiqueta Move to Archive** à política > **Salvar**.</span><span class="sxs-lookup"><span data-stu-id="32554-109">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="32554-110">Agora [atribua a Política de Retenção](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) à caixa de correio específica do utilizador.</span><span class="sxs-lookup"><span data-stu-id="32554-110">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="32554-111">A mesma política será aplicada tanto à **caixa de** correio Primária como ao **Arquivo.**</span><span class="sxs-lookup"><span data-stu-id="32554-111">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="32554-112">Pode ser necessário forçar o Assistente de Pasta Gerida (MFA) a executar e aplicar as novas definições na caixa de correio do utilizador.</span><span class="sxs-lookup"><span data-stu-id="32554-112">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="32554-113">Executar o seguinte comando enquanto [está ligado ao EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) para iniciar o Assistente de Pasta Gerida para uma caixa de correio específica:</span><span class="sxs-lookup"><span data-stu-id="32554-113">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="32554-114">Start-ManagedFolderAssistant -Identidade<name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="32554-114">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="32554-115">Para obter mais informações sobre a criação de uma política de arquivo, consulte [configurar uma política de arquivo e eliminação para caixas de correio](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="32554-115">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  