---
title: Criptografe automaticamente mensagens de correio e-mail do Office 365 enviadas para determinados domínios
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
ms.openlocfilehash: 7fb96a30cd1922bd39a4b99a7ecd869622f3a466
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/05/2021
ms.locfileid: "50526694"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a><span data-ttu-id="dfc14-102">Criptografe automaticamente mensagens de correio e-mail do Office 365 enviadas para determinados domínios</span><span class="sxs-lookup"><span data-stu-id="dfc14-102">Automatically encrypt Office 365 email messages sent to certain domains</span></span>

1. <span data-ttu-id="dfc14-103">A partir do [centro de administração Exchange,](https://outlook.office365.com/ecp/)escolha **o fluxo de correio > regras**.</span><span class="sxs-lookup"><span data-stu-id="dfc14-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="dfc14-104">Clique no ícone **Novo (+)** e, em seguida, clique **em Aplicar A encriptação de mensagens 365 e proteção de direitos para mensagens**.</span><span class="sxs-lookup"><span data-stu-id="dfc14-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="dfc14-105">Em **Nome**, introduza um nome para a regra, como *mensagens encriptadas enviadas para contoso.com*.</span><span class="sxs-lookup"><span data-stu-id="dfc14-105">In **Name**, enter a name for the rule, such as *Encrypt messages sent to contoso.com*.</span></span>
4. <span data-ttu-id="dfc14-106">Em **Aplicar esta regra se**, escolher o destinatário > domínio **é**.</span><span class="sxs-lookup"><span data-stu-id="dfc14-106">In **Apply this rule if**, choose **The recipient > domain is**.</span></span> 
5. <span data-ttu-id="dfc14-107">Insira o nome do domínio, como **contoso.com**.</span><span class="sxs-lookup"><span data-stu-id="dfc14-107">Enter the name of the domain, such as **contoso.com**.</span></span>
6. <span data-ttu-id="dfc14-108">Clique no ícone **Adicionar (+)** e, em seguida, clique **em OK**.</span><span class="sxs-lookup"><span data-stu-id="dfc14-108">Click the **Add (+)** icon, and then click **OK**.</span></span>
7. <span data-ttu-id="dfc14-109">Ao lado do campo **Fazer o seguinte,** clique **em Selecionar um**.</span><span class="sxs-lookup"><span data-stu-id="dfc14-109">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="dfc14-110">No menu drop-down **do modelo RMS,** selecione **Encrypt** e, em seguida, clique **em OK**.</span><span class="sxs-lookup"><span data-stu-id="dfc14-110">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="dfc14-111">(Se não vir esta opção, significa que o seu plano não inclui encriptação automática.</span><span class="sxs-lookup"><span data-stu-id="dfc14-111">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="dfc14-112">Mas pode adicioná-lo!)</span><span class="sxs-lookup"><span data-stu-id="dfc14-112">But you can add it!)</span></span>
9. <span data-ttu-id="dfc14-113">Escolha qualquer seleção opcional (a partir de uma lista de seleções opcionais que pode fazer neste momento, muitas das quais podem ficar com a definição padrão para a simplicidade).</span><span class="sxs-lookup"><span data-stu-id="dfc14-113">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="dfc14-114">Clique em **Guardar**.</span><span class="sxs-lookup"><span data-stu-id="dfc14-114">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="dfc14-115">Pode sempre voltar e editar esta regra mais tarde.</span><span class="sxs-lookup"><span data-stu-id="dfc14-115">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="dfc14-116">Para obter mais informações sobre a criação de regras para encriptação, consulte [Regras de fluxo de correio para encriptar mensagens de correio eletrónico no Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="dfc14-116">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>