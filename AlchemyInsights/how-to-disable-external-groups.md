---
title: Como desactivar grupos externo
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 95e60599b5298090db23bf887cb860350280964f
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/28/2019
ms.locfileid: "35384836"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="01662-102">Como desactivar grupos externo</span><span class="sxs-lookup"><span data-stu-id="01662-102">How to disable External Groups</span></span>

<span data-ttu-id="01662-103">Do Yammer mensagens externas aplicam regras de transporte de troca (ETRs), um conjunto de controlos proactivas para impedir que as informações da empresa a ser partilhado.</span><span class="sxs-lookup"><span data-stu-id="01662-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="01662-104">Para impedir que os utilizadores a criação de grupos externos, tem de configurar uma regra de transporte do Exchange (ETR) e, em seguida, do Yammer para utilizar a regra de transporte do Exchange para bloquear mensagens externas.</span><span class="sxs-lookup"><span data-stu-id="01662-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="01662-105">Depois de criar uma regra no Centro de administração Exchange Online, siga estes passos para definir ETR para aplicar no Yammer:</span><span class="sxs-lookup"><span data-stu-id="01662-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="01662-106">Iniciar sessão no Yammer como um administrador verificado e, **do Yammer Centro de administração**, vá para C **conteúdo e de segurança \> as definições de segurança.**</span><span class="sxs-lookup"><span data-stu-id="01662-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="01662-107">Em **Processamento de mensagens externo**, seleccione **impor as regras de transporte do Exchange por Exchange Online (ETRs) no Yammer.**</span><span class="sxs-lookup"><span data-stu-id="01662-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="01662-108">Selecione **Guardar**.</span><span class="sxs-lookup"><span data-stu-id="01662-108">Choose **Save**.</span></span>

<span data-ttu-id="01662-109">Para mais informações, consulte [controlo externo mensagens numa rede do Yammer com regras de transporte do Exchange](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span><span class="sxs-lookup"><span data-stu-id="01662-109">For more information, see [Control external messaging in a Yammer network with Exchange Transport rules](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span></span>
  