---
title: Impedir que as mensagens se movam automaticamente para o arquivo
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
ms.openlocfilehash: 2cb3e29dfd4f422e946b7887d4d44f373ff03794
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749824"
---
# <a name="stop-messages-from-moving-to-the-archive-automatically"></a><span data-ttu-id="e139f-102">Impedir que as mensagens se movam automaticamente para o arquivo</span><span class="sxs-lookup"><span data-stu-id="e139f-102">Stop messages from moving to the archive automatically</span></span>

<span data-ttu-id="e139f-103">Se estiver a utilizar uma política de retenção, pode alterar a idade de retenção nessa política para impedir que as mensagens arquivam automaticamente.</span><span class="sxs-lookup"><span data-stu-id="e139f-103">If you are using a retention policy, you can change the retention age in that policy to stop messages from archiving automatically.</span></span> <span data-ttu-id="e139f-104">Faça o seguinte:</span><span class="sxs-lookup"><span data-stu-id="e139f-104">Here's how:</span></span>

1. <span data-ttu-id="e139f-105">No [centro de administração Exchange,](https://go.microsoft.com/fwlink/?linkid=2059104)escolha etiquetas de retenção **de gestão de**  >  conformidade.</span><span class="sxs-lookup"><span data-stu-id="e139f-105">In the [Exchange admin center](https://go.microsoft.com/fwlink/?linkid=2059104), choose **compliance management** > **retention tags**.</span></span> <span data-ttu-id="e139f-106">Localize a sua etiqueta de retenção Move to Archive.</span><span class="sxs-lookup"><span data-stu-id="e139f-106">Locate your Move to Archive retention tag.</span></span>
2. <span data-ttu-id="e139f-107">Na etiqueta de retenção, altere o período de retenção (período de arquivo) para **nunca** impedir que os itens sejam automaticamente arquivados por uma política de retenção.</span><span class="sxs-lookup"><span data-stu-id="e139f-107">In the retention tag, change the retention period (archive period) to **Never** to stop items from being automatically archived by a retention policy.</span></span>

> [!NOTE]
> <span data-ttu-id="e139f-108">Isto altera a definição de arquivo para todas as caixas de correio com esta etiqueta de retenção aplicada a elas.</span><span class="sxs-lookup"><span data-stu-id="e139f-108">This will change the archive setting for all mailboxes with this retention tag applied to them.</span></span>
