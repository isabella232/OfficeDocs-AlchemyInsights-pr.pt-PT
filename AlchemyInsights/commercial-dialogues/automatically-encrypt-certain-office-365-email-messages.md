---
title: Criptografe automaticamente certas mensagens de correio-mail do Office 365
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: e4b2f4ffcacf03e145b4c6d5ff6e73a75cb7c184
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749441"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a><span data-ttu-id="9b8dd-102">Criptografe automaticamente certas mensagens de correio-mail do Office 365</span><span class="sxs-lookup"><span data-stu-id="9b8dd-102">Automatically encrypt certain Office 365 email messages</span></span>

<span data-ttu-id="9b8dd-103">Pode encriptar automaticamente as mensagens que os utilizadores enviam a determinadas pessoas ou organizações externas.</span><span class="sxs-lookup"><span data-stu-id="9b8dd-103">You can automatically encrypt messages that users send to certain external people or organizations.</span></span> <span data-ttu-id="9b8dd-104">Para isso, execute os seguintes passos:</span><span class="sxs-lookup"><span data-stu-id="9b8dd-104">To do this, perform the following steps:</span></span>

1. <span data-ttu-id="9b8dd-105">A partir do [centro de administração Exchange,](https://outlook.office365.com/ecp/)escolha **o fluxo de correio > regras**.</span><span class="sxs-lookup"><span data-stu-id="9b8dd-105">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="9b8dd-106">Clique no ícone **Novo (+)** e, em seguida, clique **em Aplicar A encriptação de mensagens 365 e proteção de direitos para mensagens**.</span><span class="sxs-lookup"><span data-stu-id="9b8dd-106">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="9b8dd-107">Em **Nome**, introduza um nome para a regra, como *mensagens encriptadas enviadas para DrToniRamos@gmail.com*.</span><span class="sxs-lookup"><span data-stu-id="9b8dd-107">In **Name**, enter a name for the rule, such as *Encrypt messages sent to DrToniRamos@gmail.com*.</span></span>
4. <span data-ttu-id="9b8dd-108">Em **Aplicar esta regra se**, escolher o destinatário > é esta **pessoa**.</span><span class="sxs-lookup"><span data-stu-id="9b8dd-108">In **Apply this rule if**, choose **The recipient > is this person**.</span></span> 
5. <span data-ttu-id="9b8dd-109">Na janela **'Selecionar membros',** selecione o nome da pessoa a quem deseja que a regra de encriptação se aplique e, em seguida, clique em **adicionar**.</span><span class="sxs-lookup"><span data-stu-id="9b8dd-109">In the **Select Members** window, select the name of the person you want the encryption rule to apply to, and then click **add**.</span></span> 
6. <span data-ttu-id="9b8dd-110">Quando terminar de adicionar utilizadores, clique **em OK**.</span><span class="sxs-lookup"><span data-stu-id="9b8dd-110">When you're done adding users, click **OK**.</span></span>
7. <span data-ttu-id="9b8dd-111">Ao lado do campo **Fazer o seguinte,** clique **em Selecionar um**.</span><span class="sxs-lookup"><span data-stu-id="9b8dd-111">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="9b8dd-112">No menu drop-down **do modelo RMS,** selecione **Encrypt** e, em seguida, clique **em OK**.</span><span class="sxs-lookup"><span data-stu-id="9b8dd-112">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="9b8dd-113">(Se não vir esta opção, significa que o seu plano não inclui encriptação automática.</span><span class="sxs-lookup"><span data-stu-id="9b8dd-113">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="9b8dd-114">Mas pode adicioná-lo!)</span><span class="sxs-lookup"><span data-stu-id="9b8dd-114">But you can add it!)</span></span>
9. <span data-ttu-id="9b8dd-115">Escolha qualquer seleção opcional (a partir de uma lista de seleções opcionais que pode fazer neste momento, muitas das quais podem ficar com a definição padrão para a simplicidade).</span><span class="sxs-lookup"><span data-stu-id="9b8dd-115">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="9b8dd-116">Clique em **Guardar**.</span><span class="sxs-lookup"><span data-stu-id="9b8dd-116">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="9b8dd-117">Pode sempre voltar e editar esta regra mais tarde.</span><span class="sxs-lookup"><span data-stu-id="9b8dd-117">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="9b8dd-118">Para obter mais informações sobre a criação de regras para encriptação, consulte [regras de fluxo de correio para encriptar mensagens de correio eletrónico no Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span><span class="sxs-lookup"><span data-stu-id="9b8dd-118">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span></span>

