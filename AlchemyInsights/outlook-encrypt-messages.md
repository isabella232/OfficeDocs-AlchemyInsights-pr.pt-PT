---
title: S/MIME do Outlook na web
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: f2c047ca31c586c0aa36701e6e7ca9976cfd1734
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666851"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="bbe73-102">Encriptar mensagens de correio electrónico no Outlook</span><span class="sxs-lookup"><span data-stu-id="bbe73-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="bbe73-103">Encriptação de mensagens do Office 365 foi criada no Microsoft Azure gestão de direitos (Azure RMS), que faz parte da protecção de informações de Azure.</span><span class="sxs-lookup"><span data-stu-id="bbe73-103">Office 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="bbe73-104">Se a subscrição inclui a gestão de direitos Azure ou protecção de informações Azure, **não é necessário efectuar quaisquer acções para activar manualmente ou activar** o serviço de gestão de direitos.</span><span class="sxs-lookup"><span data-stu-id="bbe73-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="bbe73-105">Com base nos comentários dos clientes, a Microsoft já não activar regras de fluxo de correio Exchange encriptar automaticamente correio electrónico enviado com determinado tipo de informações sensíveis no seu tenant por predefinição.</span><span class="sxs-lookup"><span data-stu-id="bbe73-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="bbe73-106">Em vez disso, estamos a fornecer instruções detalhadas sobre como pode fazê-lo mitos.</span><span class="sxs-lookup"><span data-stu-id="bbe73-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="bbe73-107">Para obter detalhes adicionais sobre como criar uma regra de transporte para encriptar informações sensíveis, consulte [Este artigo](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="bbe73-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="bbe73-108">Se utilizar o Outlook na Web (anteriormente **OWA**): quando estiver a compor uma mensagem de correio electrónico, basta clicar **proteger** no OWA.</span><span class="sxs-lookup"><span data-stu-id="bbe73-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="bbe73-109">Isto aplicará a permissão "Não reencaminhar".</span><span class="sxs-lookup"><span data-stu-id="bbe73-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="bbe73-110">Clique em **Alterar permissão** e escolher **encriptar** apenas a encriptar a mensagem.</span><span class="sxs-lookup"><span data-stu-id="bbe73-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="bbe73-111">Se utilizar o **cliente Outlook**: para enviar uma mensagem encriptada a partir do Outlook 2013 ou de 2016, ou de 2016 do Outlook para Mac, seleccione **Opções** > **permissões**, em seguida, seleccione a opção de protecção que necessita.</span><span class="sxs-lookup"><span data-stu-id="bbe73-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="bbe73-112">Para **encriptar automaticamente todas as mensagem de correio electrónico** enviadas para determinados destinatários ou organizações de parceiro externo, é necessário criar uma regra de transporte de fluxo de correio no Centro de administração do Exchange.</span><span class="sxs-lookup"><span data-stu-id="bbe73-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="bbe73-113">São fornecidas instruções detalhadas no [presente artigo de suporte](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="bbe73-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

