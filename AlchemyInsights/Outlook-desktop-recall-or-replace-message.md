---
title: Outlook Desktop recall ou substituir uma mensagem de e-mail
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 3d3a6c253317137b7069a978b907c97d61bf7313
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/15/2019
ms.locfileid: "36496122"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="4a212-102">Lembre-se ou substitua uma mensagem de e-mail do Outlook</span><span class="sxs-lookup"><span data-stu-id="4a212-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="4a212-103">Como administrador, você pode **recordar mensagens em nome dos usuários usando powershell**.</span><span class="sxs-lookup"><span data-stu-id="4a212-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="4a212-104">Você não pode se lembrar de mensagens do centro de administração.</span><span class="sxs-lookup"><span data-stu-id="4a212-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="4a212-105">Você só pode **recordar mensagens que são enviadas para as pessoas em sua organização**.</span><span class="sxs-lookup"><span data-stu-id="4a212-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="4a212-106">Se a mensagem foi enviada para um endereço do Gmail, por exemplo, você não pode se lembrar.</span><span class="sxs-lookup"><span data-stu-id="4a212-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="4a212-107">Você só pode **recordar as mensagens enviadas do Outlook 2016 no PC**.</span><span class="sxs-lookup"><span data-stu-id="4a212-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="4a212-108">Se um usuário enviar uma mensagem usando o Outlook para Mac ou Outlook na web, você não pode se lembrar.</span><span class="sxs-lookup"><span data-stu-id="4a212-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="4a212-109">Para recordar ou substituir uma mensagem de e-mail:</span><span class="sxs-lookup"><span data-stu-id="4a212-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="4a212-110">No painel de pasta à esquerda da janela do Outlook, selecione a pasta Sent Items.</span><span class="sxs-lookup"><span data-stu-id="4a212-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="4a212-111">Clique duas vezes na mensagem que deseja recordar para abri-la.</span><span class="sxs-lookup"><span data-stu-id="4a212-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="4a212-112">Selecione a guia **mensagem** e, em seguida, selecione **ações** > **lembrem essa mensagem**.</span><span class="sxs-lookup"><span data-stu-id="4a212-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="4a212-113">Selecione **excluir cópias não lidas desta mensagem** ou excluir **cópias não lidas e substituir por uma nova mensagem,** e, em seguida, selecione **OK**.</span><span class="sxs-lookup"><span data-stu-id="4a212-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="4a212-114">Se você estiver enviando uma mensagem de substituição, componha a mensagem e selecione **envie.**</span><span class="sxs-lookup"><span data-stu-id="4a212-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="4a212-115">O sucesso ou o fracasso de um recall de mensagens depende das configurações do destinatário no Outlook.</span><span class="sxs-lookup"><span data-stu-id="4a212-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="4a212-116">Para que as etapas verific na recordação, veja [este artigo.](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)</span><span class="sxs-lookup"><span data-stu-id="4a212-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="4a212-117">Pesquise e exclua mensagens de e-mail em sua organização</span><span class="sxs-lookup"><span data-stu-id="4a212-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="4a212-118">Se você não for um administrador global, sua conta deve ser adicionada à função do gerente do eDiscovery ou à função de gerenciamento de pesquisa de conformidade para pesquisar mensagens.</span><span class="sxs-lookup"><span data-stu-id="4a212-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="4a212-119">Para excluir mensagens, você precisará participar do grupo de função da Organização Gerencial ou da função de gerenciamento de Pesquisa e Expurgo.</span><span class="sxs-lookup"><span data-stu-id="4a212-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="4a212-120">As permissões para essas funções são atribuídas no centro de [segurança e conformidade.](https://go.microsoft.com/fwlink/?linkid=2083731)</span><span class="sxs-lookup"><span data-stu-id="4a212-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="4a212-121">[Crie uma pesquisa de conteúdo](https://docs.microsoft.com/office365/securitycompliance/content-search) para encontrar a mensagem para excluir.</span><span class="sxs-lookup"><span data-stu-id="4a212-121">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="4a212-122">[Conecte-se ao PowerShell do Centro](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)de Segurança e Conformidade.</span><span class="sxs-lookup"><span data-stu-id="4a212-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="4a212-123">Se você estiver usando a autenticação multifator, [consulte o Connect to Office 365 Security and Compliance Center PowerShell usando autenticação multifator.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="4a212-123">If you're using multi-factor authentication, see [Connect to Office 365 Security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>