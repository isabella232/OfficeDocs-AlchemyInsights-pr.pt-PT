---
title: Outlook Desktop recordação ou substitui uma mensagem de e-mail
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 578e2690061286bde74ee0b4b74a197630716f59
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664001"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="9c79b-102">Relembrou substituir uma mensagem de email do Outlook</span><span class="sxs-lookup"><span data-stu-id="9c79b-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="9c79b-103">Como administrador, pode **recordar mensagens em nome dos utilizadores que utilizam o PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="9c79b-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="9c79b-104">Não se lembra das mensagens do centro de administração.</span><span class="sxs-lookup"><span data-stu-id="9c79b-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="9c79b-105">Só se **pode recordar mensagens enviadas a pessoas da sua organização.**</span><span class="sxs-lookup"><span data-stu-id="9c79b-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="9c79b-106">Se a mensagem foi enviada para um endereço Gmail, por exemplo, não se lembra.</span><span class="sxs-lookup"><span data-stu-id="9c79b-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="9c79b-107">Só é **possível recordar as mensagens enviadas do Outlook 2016 no PC**.</span><span class="sxs-lookup"><span data-stu-id="9c79b-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="9c79b-108">Se um utilizador enviar uma mensagem utilizando o Outlook for Mac ou Outlook na web, não se pode lembrar dela.</span><span class="sxs-lookup"><span data-stu-id="9c79b-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="9c79b-109">Para recordar ou substituir uma mensagem de e-mail:</span><span class="sxs-lookup"><span data-stu-id="9c79b-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="9c79b-110">No painel de pastas à esquerda da janela Outlook, selecione a pasta 'Itens Enviados'.</span><span class="sxs-lookup"><span data-stu-id="9c79b-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="9c79b-111">Clique duas vezes na mensagem que deseja recordar para abri-la.</span><span class="sxs-lookup"><span data-stu-id="9c79b-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="9c79b-112">Selecione o separador **Mensagem** e, em seguida, selecione **Ações**  >  **Relembrem esta mensagem**.</span><span class="sxs-lookup"><span data-stu-id="9c79b-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="9c79b-113">**Selecione Eliminar cópias não lidas desta mensagem** ou **eliminar cópias não lidas e substituir por uma nova mensagem**e, em seguida, selecione **OK**.</span><span class="sxs-lookup"><span data-stu-id="9c79b-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="9c79b-114">Se estiver a enviar uma mensagem de substituição, compõe a mensagem e, em seguida, selecione **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="9c79b-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="9c79b-115">O sucesso ou falha de uma chamada de mensagem depende das definições do destinatário no Outlook.</span><span class="sxs-lookup"><span data-stu-id="9c79b-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="9c79b-116">Para obter medidas para verificar a recolha, consulte [este artigo](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="9c79b-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="9c79b-117">Procure e elimine mensagens de e-mail na sua organização</span><span class="sxs-lookup"><span data-stu-id="9c79b-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="9c79b-118">Se não for administrador global, a sua conta tem de ser adicionada à função de Gestor de EDiscovery ou à função de gestão de Compliance Search para procurar mensagens.</span><span class="sxs-lookup"><span data-stu-id="9c79b-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="9c79b-119">Para eliminar mensagens, terá de se juntar ao grupo de funções de Gestão da Organização ou à função de gestão de Pesquisa e Purga.</span><span class="sxs-lookup"><span data-stu-id="9c79b-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="9c79b-120">As permissões para estas funções são atribuídas no [Centro de Segurança e Conformidade](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="9c79b-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="9c79b-121">[Crie uma pesquisa de conteúdo](https://docs.microsoft.com/microsoft-365/compliance/content-search) para encontrar a mensagem para eliminar.</span><span class="sxs-lookup"><span data-stu-id="9c79b-121">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="9c79b-122">[Ligue-se ao Centro de Segurança e Conformidade PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="9c79b-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="9c79b-123">Se estiver a utilizar a autenticação multi-factor, consulte [Connect to Microsoft 365 security and Compliance Center PowerShell utilizando a autenticação de vários fatores](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="9c79b-123">If you're using multi-factor authentication, see [Connect to Microsoft 365 security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>