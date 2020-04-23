---
title: Como desativar grupos externos
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 2159feb4aa3999072de57d76790a2959c7355976
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720779"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="53547-102">Como desativar grupos externos</span><span class="sxs-lookup"><span data-stu-id="53547-102">How to disable External Groups</span></span>

<span data-ttu-id="53547-103">As mensagens externas yammer aplicam regras de transporte de câmbio (ETRs), um conjunto de controlos proactivos para impedir que as informações da empresa sejam partilhadas.</span><span class="sxs-lookup"><span data-stu-id="53547-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="53547-104">Para restringir os utilizadores à criação de grupos externos, é necessário configurar uma regra de transporte de intercâmbio (ETR) e, em seguida, configurar a Yammer para usar a regra de Transporte de Intercâmbio para bloquear mensagens externas.</span><span class="sxs-lookup"><span data-stu-id="53547-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="53547-105">Depois de ter criado uma regra no centro de administração Exchange Online, siga estes passos para definir o ETR para aplicar em Yammer:</span><span class="sxs-lookup"><span data-stu-id="53547-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="53547-106">Inicie sessão na Yammer como administrador verificado, e no centro de **administração yammer,** aceda às Definições de \*\*Segurança de Conteúdo C e Segurança. \> \*\*</span><span class="sxs-lookup"><span data-stu-id="53547-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="53547-107">Sob **mensagens externas,** selecione Faça cumprir as suas Regras de Transporte de **Intercâmbio Online (ETRs) em Yammer.**</span><span class="sxs-lookup"><span data-stu-id="53547-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="53547-108">Selecione **Guardar**.</span><span class="sxs-lookup"><span data-stu-id="53547-108">Choose **Save**.</span></span>

<span data-ttu-id="53547-109">Para mais informações, consulte [Desativar mensagens externas numa rede Yammer](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span><span class="sxs-lookup"><span data-stu-id="53547-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  