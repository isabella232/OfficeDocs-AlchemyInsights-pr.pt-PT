---
title: Mover automaticamente mensagens de correio eletrónico para a caixa de correio de arquivo
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 14ded561ee2b3c244fadbdab42fd0e833a1c66d5
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749285"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a><span data-ttu-id="8389f-102">Mover automaticamente mensagens de correio eletrónico para a caixa de correio de arquivo</span><span class="sxs-lookup"><span data-stu-id="8389f-102">Automatically move email messages to the archive mailbox</span></span>

<span data-ttu-id="8389f-103">Eis como configurar uma política para mover automaticamente o antigo e-mail de um utilizador para a caixa de correio de arquivo:</span><span class="sxs-lookup"><span data-stu-id="8389f-103">Here's how to set up a policy to automatically move a user's old email to the archive mailbox:</span></span>

1. <span data-ttu-id="8389f-104">Vá ao [**Security & Compliance**](https://go.microsoft.com/fwlink/p/?linkid=2077143)Data Governance Archive para verificar se uma caixa de correio de arquivo foi  >    >   ativada para o utilizador.</span><span class="sxs-lookup"><span data-stu-id="8389f-104">Go to [**Security & Compliance**](https://go.microsoft.com/fwlink/p/?linkid=2077143) > **Data governance** > **Archive** to verify an archive mailbox has been enabled for the user.</span></span> <span data-ttu-id="8389f-105">Se não tiver, clique em **Ativar** então **Sim** na caixa de aviso.</span><span class="sxs-lookup"><span data-stu-id="8389f-105">If it hasn't, click **Enable** then **Yes** in the warning box.</span></span>
2. <span data-ttu-id="8389f-106">Vá ao [**Centro de Administração Exchange > etiquetas de gestão de conformidade > de retenção.**](https://go.microsoft.com/fwlink/?linkid=2059104)</span><span class="sxs-lookup"><span data-stu-id="8389f-106">Go to [**Exchange admin center > compliance management > retention tags**](https://go.microsoft.com/fwlink/?linkid=2059104).</span></span>
3. <span data-ttu-id="8389f-107">Escolha o ícone + e escolha **aplicar-se automaticamente a toda a caixa de correio.**</span><span class="sxs-lookup"><span data-stu-id="8389f-107">Choose the + icon then choose **automatically apply to entire mailbox**.</span></span>
4. <span data-ttu-id="8389f-108">Atribua um nome à etiqueta de retenção e escolha **Mover to Archive**.</span><span class="sxs-lookup"><span data-stu-id="8389f-108">Assign a name to the retention tag, and choose **Move to Archive**.</span></span> <span data-ttu-id="8389f-109">Para o período de retenção, insira o tempo que quiser, como 90 dias.</span><span class="sxs-lookup"><span data-stu-id="8389f-109">For the retention period, enter the time you want, such as 90 days.</span></span> <span data-ttu-id="8389f-110">Clique em **Guardar**.</span><span class="sxs-lookup"><span data-stu-id="8389f-110">Click **Save**.</span></span>
5. <span data-ttu-id="8389f-111">Agora crie uma política de retenção: escolha **políticas de retenção,** escolha o ícone para adicionar uma nova política.</span><span class="sxs-lookup"><span data-stu-id="8389f-111">Now create a retention policy: choose **retention policies**, choose the icon to add a new policy.</span></span>
6. <span data-ttu-id="8389f-112">Atribua um nome à política de retenção, clique e percorra para encontrar e adicionar a etiqueta de retenção que acabou de criar.</span><span class="sxs-lookup"><span data-stu-id="8389f-112">Assign a name to the retention policy, then click and scroll to find and add the retention tag you just created.</span></span> <span data-ttu-id="8389f-113">Clique em **Guardar**.</span><span class="sxs-lookup"><span data-stu-id="8389f-113">Click **Save**.</span></span>
7. <span data-ttu-id="8389f-114">Por fim, aplique a política de retenção na caixa de correio do utilizador: ainda no centro de administração Exchange, vá às caixas de correio **dos**  >  **destinatários**.</span><span class="sxs-lookup"><span data-stu-id="8389f-114">Finally, apply the retention policy to the user's mailbox: still in the Exchange admin center, go to **recipients** > **mailboxes**.</span></span> <span data-ttu-id="8389f-115">Escolha todos os utilizadores a quem pretende aplicar a política e, em seguida, escolha **Editar** (o ícone do lápis).</span><span class="sxs-lookup"><span data-stu-id="8389f-115">Choose all the users who you want to apply the policy to, then choose **Edit** (the pencil icon).</span></span>
8. <span data-ttu-id="8389f-116">Na caixa de diálogo, clique nas **funcionalidades da caixa de correio**.</span><span class="sxs-lookup"><span data-stu-id="8389f-116">In the dialog box, click **mailbox features**.</span></span> <span data-ttu-id="8389f-117">No âmbito **da política de retenção,** aplique a política que acabou de criar > **Salvar**.</span><span class="sxs-lookup"><span data-stu-id="8389f-117">Under **Retention policy**, apply the policy you just created > **Save**.</span></span>
9. <span data-ttu-id="8389f-118">Para obter instruções para aplicar a apólice a todos os utilizadores, consulte [Aplicar uma política de retenção nas caixas de correio](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).</span><span class="sxs-lookup"><span data-stu-id="8389f-118">For instructions for applying the policy to all users, see [Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).</span></span>
