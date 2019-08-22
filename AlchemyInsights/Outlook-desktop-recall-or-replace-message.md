---
title: Resgate de ambiente de trabalho do Outlook ou substituir uma mensagem de correio electrónico
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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36496122"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="50beb-102">Resgatar ou substituir uma mensagem de correio electrónico do Outlook</span><span class="sxs-lookup"><span data-stu-id="50beb-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="50beb-103">Como administrador, pode de **resgate de mensagens em nome dos utilizadores utilizando o PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="50beb-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="50beb-104">Não é possível recuperar mensagens a partir do Centro de administração.</span><span class="sxs-lookup"><span data-stu-id="50beb-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="50beb-105">Pode **apenas mensagens de recuperação que são enviadas para pessoas na organização**.</span><span class="sxs-lookup"><span data-stu-id="50beb-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="50beb-106">Se a mensagem foi enviada para um endereço de Gmail, por exemplo, não se lembrá-lo.</span><span class="sxs-lookup"><span data-stu-id="50beb-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="50beb-107">Pode **apenas resgatar as mensagens enviadas de 2016 do Outlook no computador**.</span><span class="sxs-lookup"><span data-stu-id="50beb-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="50beb-108">Se um utilizador envia uma mensagem utilizando o Outlook para Mac ou o Outlook na web, não se lembrá-lo.</span><span class="sxs-lookup"><span data-stu-id="50beb-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="50beb-109">Para resgatar ou substituir uma mensagem de correio electrónico:</span><span class="sxs-lookup"><span data-stu-id="50beb-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="50beb-110">No painel de pastas do lado esquerdo da janela do Outlook, seleccione a pasta Itens enviados.</span><span class="sxs-lookup"><span data-stu-id="50beb-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="50beb-111">Faça duplo clique sobre a mensagem que pretende recuperar para o abrir.</span><span class="sxs-lookup"><span data-stu-id="50beb-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="50beb-112">Seleccione o separador de **mensagem** e, em seguida, seleccione **Acções** > **Resgatar a mensagem**.</span><span class="sxs-lookup"><span data-stu-id="50beb-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="50beb-113">Seleccione **Eliminar cópias não lidas desta mensagem** ou **elimine cópias não lidas e substitua por uma nova mensagem**e, em seguida, seleccione **' OK '**.</span><span class="sxs-lookup"><span data-stu-id="50beb-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="50beb-114">Se estiver a enviar uma mensagem de substituição, compor a mensagem e, em seguida, seleccione **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="50beb-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="50beb-115">O êxito ou falha do resgate de mensagens depende de definições do destinatário do Outlook.</span><span class="sxs-lookup"><span data-stu-id="50beb-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="50beb-116">Para obter passos verificar a recuperação, consulte [Este artigo](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="50beb-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="50beb-117">Procure e elimine mensagens de correio electrónico na organização</span><span class="sxs-lookup"><span data-stu-id="50beb-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="50beb-118">Se não for um administrador global, a conta deve ser adicionada à função de Gestor de detecção de dados electrónicos ou a função de gestão de conformidade Procurar para procurar mensagens.</span><span class="sxs-lookup"><span data-stu-id="50beb-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="50beb-119">Para eliminar mensagens, terá de associar o grupo de funções de gestão da organização ou a função de gestão de procura e remover.</span><span class="sxs-lookup"><span data-stu-id="50beb-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="50beb-120">Permissões para estas funções são atribuídas no [Centro de segurança e conformidade](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="50beb-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="50beb-121">[Criar um conteúdo de procura](https://docs.microsoft.com/office365/securitycompliance/content-search) para localizar a mensagem para eliminar.</span><span class="sxs-lookup"><span data-stu-id="50beb-121">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="50beb-122">[Ligar a segurança e conformidade Centro PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="50beb-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="50beb-123">Se estiver a utilizar autenticação multi-factores, consulte [ligar para a segurança do Office 365 e conformidade Centro PowerShell utilizando autenticação multi-factores](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="50beb-123">If you're using multi-factor authentication, see [Connect to Office 365 Security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>