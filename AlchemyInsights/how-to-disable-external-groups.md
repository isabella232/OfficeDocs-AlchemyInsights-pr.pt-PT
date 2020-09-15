---
title: Como desativar grupos externos
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: f7a1bbda3a54d2662bdfe21cda961c32456edb82
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704139"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="38b7a-102">Como desativar grupos externos</span><span class="sxs-lookup"><span data-stu-id="38b7a-102">How to disable External Groups</span></span>

<span data-ttu-id="38b7a-103">A mensagem externa da Yammer aplica regras de transporte de câmbio (ETRs), um conjunto de controlos pró-ativos para impedir que a informação da empresa seja partilhada.</span><span class="sxs-lookup"><span data-stu-id="38b7a-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="38b7a-104">Para restringir os utilizadores à criação de grupos externos, é necessário configurar uma regra de transporte de intercâmbio (ETR) e, em seguida, configurar a Yammer para usar a regra do Transporte de Intercâmbio para bloquear mensagens externas.</span><span class="sxs-lookup"><span data-stu-id="38b7a-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="38b7a-105">Uma vez criada uma regra no Centro de Administração Exchange Online, siga estes passos para definir ETR para aplicar em Yammer:</span><span class="sxs-lookup"><span data-stu-id="38b7a-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="38b7a-106">Inicie sessão no Yammer como administrador verificado, e no **centro de administração Yammer,** vá para C **Conteúdo e \> Definições de Segurança.**</span><span class="sxs-lookup"><span data-stu-id="38b7a-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="38b7a-107">Em **Mensagens Externas,** **selecione Impor as suas Regras de Transporte de Intercâmbio Online (ETRs) em Yammer.**</span><span class="sxs-lookup"><span data-stu-id="38b7a-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="38b7a-108">Selecione **Guardar**.</span><span class="sxs-lookup"><span data-stu-id="38b7a-108">Choose **Save**.</span></span>

<span data-ttu-id="38b7a-109">Para obter mais informações, consulte [Mensagens externas desativada numa rede Yammer](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span><span class="sxs-lookup"><span data-stu-id="38b7a-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  