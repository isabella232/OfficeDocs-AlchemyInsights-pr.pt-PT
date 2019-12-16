---
title: S/MIME em Outlook na web
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 33e94eac6a2982b8036e13d17bf60015f244f2cb
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053236"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="1f8bc-102">Criptografar mensagens de e-mail no Outlook</span><span class="sxs-lookup"><span data-stu-id="1f8bc-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="1f8bc-103">A criptografia de mensagens do Office 365 é construída no Microsoft Azure Rights Management (Azure RMS), que faz parte da Proteção de Informações do Azure.</span><span class="sxs-lookup"><span data-stu-id="1f8bc-103">Office 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="1f8bc-104">Se sua assinatura incluir a Gestão de Direitos Do Azure ou a Proteção de Informações do Azure, **você não precisará tomar nenhuma ação para ativar ou ativar manualmente** o Serviço de Gerenciamento de Direitos.</span><span class="sxs-lookup"><span data-stu-id="1f8bc-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="1f8bc-105">Com base no feedback do cliente, não estaremos mais permitindo que as regras de fluxo de e-mail da Exchange criptografem automaticamente o e-mail de saída contendo determinado tipo de informação sensível em seu locatário por padrão.</span><span class="sxs-lookup"><span data-stu-id="1f8bc-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="1f8bc-106">Em vez disso, estamos fornecendo instruções detalhadas sobre como você pode fazê-lo sozinhos.</span><span class="sxs-lookup"><span data-stu-id="1f8bc-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="1f8bc-107">Para obter detalhes adicionais sobre como criar uma regra de transporte para criptografar informações confidenciais, consulte [este artigo.](https://aka.ms/OmeEtr)</span><span class="sxs-lookup"><span data-stu-id="1f8bc-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="1f8bc-108">Se estiver usando o Outlook na Web (anteriormente **OWA):** Ao compor uma mensagem de e-mail, basta clicar em **Proteger** na OWA.</span><span class="sxs-lookup"><span data-stu-id="1f8bc-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="1f8bc-109">Isso aplicará a permissão "Não encaminhe".</span><span class="sxs-lookup"><span data-stu-id="1f8bc-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="1f8bc-110">Clique **na permissão de alteração** e escolha **criptografar** apenas a mensagem.</span><span class="sxs-lookup"><span data-stu-id="1f8bc-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="1f8bc-111">Se estiver usando o **cliente do Outlook:** Para enviar uma mensagem criptografada do Outlook 2013 ou 2016, ou Outlook 2016 para Mac, selecione**Permissões**de **Opções** > e selecione a opção de proteção de que precisa.</span><span class="sxs-lookup"><span data-stu-id="1f8bc-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="1f8bc-112">Para **criptografar automaticamente todos os e-mails** enviados a determinados destinatários ou organizações parceiras externas, você precisa criar uma regra de transporte de fluxo de correio no Exchange Admin Center.</span><span class="sxs-lookup"><span data-stu-id="1f8bc-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="1f8bc-113">Instruções detalhadas são fornecidas [neste artigo de suporte.](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities)</span><span class="sxs-lookup"><span data-stu-id="1f8bc-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

