---
title: Como desactivar grupos externo
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 4d911c319c3e8e327f9b3af3ba67816e646bc468
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/12/2019
ms.locfileid: "29899147"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="6d71e-102">Como desactivar grupos externo</span><span class="sxs-lookup"><span data-stu-id="6d71e-102">How to disable External Groups</span></span>

<span data-ttu-id="6d71e-p101">Do Yammer mensagens externas aplicam regras de transporte de troca (ETRs), um conjunto de controlos proactivas para impedir que as informações da empresa a ser partilhado. Para impedir que os utilizadores a criação de grupos externos, tem de configurar uma regra de transporte do Exchange (ETR) e, em seguida, do Yammer para utilizar a regra de transporte do Exchange para bloquear mensagens externas.</span><span class="sxs-lookup"><span data-stu-id="6d71e-p101">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared. In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span> 
  
<span data-ttu-id="6d71e-105">Depois de criar uma regra no Centro de administração Exchange Online, siga estes passos para definir ETR para aplicar no Yammer:</span><span class="sxs-lookup"><span data-stu-id="6d71e-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="6d71e-106">Iniciar sessão no Yammer como um administrador verificado e, **do Yammer Centro de administração**, vá para C **onteúdo e de segurança \> as definições de segurança.**</span><span class="sxs-lookup"><span data-stu-id="6d71e-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **ontent and Security \> Security Settings.**</span></span>
    
- <span data-ttu-id="6d71e-107">Em **Processamento de mensagens externo**, seleccione **impor as regras de transporte do Exchange por Exchange Online (ETRs) no Yammer.**</span><span class="sxs-lookup"><span data-stu-id="6d71e-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>
    
- <span data-ttu-id="6d71e-108">Selecione **Save**.</span><span class="sxs-lookup"><span data-stu-id="6d71e-108">Choose **Save**.</span></span> 
    
<span data-ttu-id="6d71e-109">Para mais informações, consulte [controlo externo mensagens numa rede do Yammer com regras de transporte do Exchange](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span><span class="sxs-lookup"><span data-stu-id="6d71e-109">For more information, see [Control external messaging in a Yammer network with Exchange Transport rules](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span></span>
  

