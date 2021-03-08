---
title: Criptografe automaticamente certas mensagens de correio e-mail do escritório 365
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
ms.openlocfilehash: 5ddaaed361f6ec934cfffb00cc62a9df2d1a04e8
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/05/2021
ms.locfileid: "50526760"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a><span data-ttu-id="587b9-102">Criptografe automaticamente certas mensagens de correio e-mail do escritório 365</span><span class="sxs-lookup"><span data-stu-id="587b9-102">Automatically encrypt certain email messages from office 365</span></span>

1. <span data-ttu-id="587b9-103">A partir do [centro de administração Exchange,](https://outlook.office365.com/ecp/)escolha **o fluxo de correio > regras**.</span><span class="sxs-lookup"><span data-stu-id="587b9-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="587b9-104">Clique no ícone **Novo (+)** e, em seguida, clique **em Aplicar A encriptação de mensagens 365 e proteção de direitos para mensagens**.</span><span class="sxs-lookup"><span data-stu-id="587b9-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="587b9-105">Em **Nome**, introduza um nome para a regra, como *encriptar todas as mensagens*.</span><span class="sxs-lookup"><span data-stu-id="587b9-105">In **Name**, enter a name for the rule, such as *Encrypt all messages*.</span></span>
4. <span data-ttu-id="587b9-106">Em **Aplicar esta regra se,** escolher **[Aplicar a todas as mensagens]**.</span><span class="sxs-lookup"><span data-stu-id="587b9-106">In **Apply this rule if**, choose **[Apply to all messages]**.</span></span> 
5. <span data-ttu-id="587b9-107">Ao lado do campo **Fazer o seguinte,** clique **em Selecionar um**.</span><span class="sxs-lookup"><span data-stu-id="587b9-107">Next to the **Do the following** field, click **Select one**.</span></span> 
6. <span data-ttu-id="587b9-108">No menu drop-down **do modelo RMS,** selecione **Encrypt** e, em seguida, clique **em OK**.</span><span class="sxs-lookup"><span data-stu-id="587b9-108">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="587b9-109">(Se não vir esta opção, significa que o seu plano não inclui encriptação automática.</span><span class="sxs-lookup"><span data-stu-id="587b9-109">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="587b9-110">Mas pode adicioná-lo!)</span><span class="sxs-lookup"><span data-stu-id="587b9-110">But you can add it!)</span></span>
7. <span data-ttu-id="587b9-111">Verifique a Auditoria esta regra com caixa **de verificação de nível de severidade** e, em seguida, selecione o nível pretendido.</span><span class="sxs-lookup"><span data-stu-id="587b9-111">Check the **Audit this rule with severity level** check box, and then select the desired level.</span></span> <span data-ttu-id="587b9-112">Se a sua empresa tiver obrigações contratuais para enviar todos os e-mails encriptados, recomendo definir o nível para **High**.</span><span class="sxs-lookup"><span data-stu-id="587b9-112">If your company has contractual obligations to send all emails encrypted, I recommend setting the level to **High**.</span></span>
8. <span data-ttu-id="587b9-113">Em **Escolha um modelo para esta regra,** clique em **Enforce**.</span><span class="sxs-lookup"><span data-stu-id="587b9-113">Under **Choose a model for this rule**, click **Enforce**.</span></span> 
9. <span data-ttu-id="587b9-114">Escolha qualquer seleção opcional (a partir de uma lista de seleções opcionais que pode fazer neste momento, muitas das quais podem ficar com a definição padrão para a simplicidade).</span><span class="sxs-lookup"><span data-stu-id="587b9-114">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="587b9-115">Clique em **Guardar**.</span><span class="sxs-lookup"><span data-stu-id="587b9-115">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="587b9-116">Pode sempre voltar e editar esta regra mais tarde.</span><span class="sxs-lookup"><span data-stu-id="587b9-116">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="587b9-117">Para obter mais informações sobre a criação de regras para encriptação, consulte [Regras de fluxo de correio para encriptar mensagens de correio eletrónico no Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="587b9-117">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>

