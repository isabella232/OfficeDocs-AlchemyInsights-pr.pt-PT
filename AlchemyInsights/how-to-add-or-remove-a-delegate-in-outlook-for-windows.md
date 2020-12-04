---
title: Como adicionar ou remover um delegado no Outlook para windows
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800004"
- "7334"
ms.openlocfilehash: fcbd6082c104f0e1bca022a23cbbeb6e3363a6c5
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573574"
---
# <a name="how-to-add-or-remove-a-delegate-in-outlook-for-windows"></a><span data-ttu-id="c113c-102">Como adicionar ou remover um delegado no Outlook para windows</span><span class="sxs-lookup"><span data-stu-id="c113c-102">How to add or remove a Delegate in Outlook for Windows</span></span>

<span data-ttu-id="c113c-103">Para adicionar um delegado no Outlook for Windows:</span><span class="sxs-lookup"><span data-stu-id="c113c-103">To add a Delegate in Outlook for Windows:</span></span> 

1. <span data-ttu-id="c113c-104">Clique no **separador Ficheiro** seguido de **Definições de Conta** e, em seguida, escolha O Acesso **delegado**.</span><span class="sxs-lookup"><span data-stu-id="c113c-104">Click on the **File** tab followed by **Account Settings**, and then choose **Delegate Access**.</span></span>
2. <span data-ttu-id="c113c-105">Clique em **Adicionar**.</span><span class="sxs-lookup"><span data-stu-id="c113c-105">Click on **Add**.</span></span> <span data-ttu-id="c113c-106">Se **o Add** não aparecer, pode não existir uma ligação ativa entre o Outlook e o Exchange.</span><span class="sxs-lookup"><span data-stu-id="c113c-106">If **Add** doesn’t appear, an active connection might not exist between Outlook and Exchange.</span></span> <span data-ttu-id="c113c-107">A barra de estado do Outlook apresenta o estado de ligação.</span><span class="sxs-lookup"><span data-stu-id="c113c-107">The Outlook status bar displays the connection status.</span></span>
3. <span data-ttu-id="c113c-108">Digite o nome da pessoa que pretende designar como seu delegado, ou procure e escolha o nome na lista de resultados de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="c113c-108">Type the name of the person you want to designate as your delegate, or search and choose the name in the search results list.</span></span>

    > [!NOTE]
    > <span data-ttu-id="c113c-109">O delegado deve ser uma pessoa na Lista de Endereços Globais da sua organização (GAL).</span><span class="sxs-lookup"><span data-stu-id="c113c-109">The delegate must be a person in your organization's Exchange Global Address List (GAL).</span></span>
4. <span data-ttu-id="c113c-110">Clique em **Adicionar** seguido por **OK**.</span><span class="sxs-lookup"><span data-stu-id="c113c-110">Click on **Add** followed by **OK**.</span></span>
5. <span data-ttu-id="c113c-111">Na caixa de diálogo **Dedesemesta permissões,** aceite as definições de permissão predefinidos ou selecione níveis de acesso personalizados para pastas De troca.</span><span class="sxs-lookup"><span data-stu-id="c113c-111">In the **Delegate Permissions** dialog box, accept the default permission settings or select custom access levels for Exchange folders.</span></span>

    - <span data-ttu-id="c113c-112">Se um delegado precisar de permissão para trabalhar apenas com pedidos e respostas de reunião, as definições de permissão por defeito, como **delegado, recebem cópias de mensagens relacionadas com a reunião enviadas para mim são suficientes.**</span><span class="sxs-lookup"><span data-stu-id="c113c-112">If a delegate needs permission to work only with meeting requests and responses, the default permission settings such as **Delegate receives copies of meeting-related messages sent to me** are sufficient.</span></span> <span data-ttu-id="c113c-113">Pode deixar a definição de permissão **de caixa de** entrada em **Nenhum**.</span><span class="sxs-lookup"><span data-stu-id="c113c-113">You can leave the **Inbox** permission setting at **None**.</span></span> <span data-ttu-id="c113c-114">Os pedidos e respostas da reunião irão diretamente para a caixa de entrada do delegado.</span><span class="sxs-lookup"><span data-stu-id="c113c-114">Meeting requests and responses will go directly to the delegate's inbox.</span></span>

    > [!NOTE]
    > <span data-ttu-id="c113c-115">Por predefinição, o delegado recebe permissão **do Editor (pode ler, criar e modificar itens)** para a sua pasta **Calendar.**</span><span class="sxs-lookup"><span data-stu-id="c113c-115">By default, the delegate is granted **Editor (can read, create, and modify items)** permission to your **Calendar** folder.</span></span> <span data-ttu-id="c113c-116">Quando o delegado responde a uma reunião em seu nome, é automaticamente adicionado à sua pasta **Calendar.**</span><span class="sxs-lookup"><span data-stu-id="c113c-116">When the delegate responds to a meeting on your behalf, it is automatically added to your **Calendar** folder.</span></span>

5. <span data-ttu-id="c113c-117">Para enviar uma mensagem para notificar o delegado das permissões alteradas, selecione a **enviar automaticamente uma mensagem para delegar resumindo a caixa de verificação destas permissões.**</span><span class="sxs-lookup"><span data-stu-id="c113c-117">To send a message to notify the delegate of the changed permissions, select the **Automatically send a message to delegate summarizing these permissions** check box.</span></span>
6. <span data-ttu-id="c113c-118">Se quiser, selecione o Delegado pode ver a minha caixa de verificação **de itens privados.**</span><span class="sxs-lookup"><span data-stu-id="c113c-118">If you want, select the **Delegate can see my private items** check box.</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="c113c-119">Esta definição afeta todas as pastas Exchange.</span><span class="sxs-lookup"><span data-stu-id="c113c-119">This setting affects all Exchange folders.</span></span> <span data-ttu-id="c113c-120">Isto inclui todas as pastas de Correio, Contactos, Calendário, Tarefas, Notas e Diário.</span><span class="sxs-lookup"><span data-stu-id="c113c-120">This includes all Mail, Contacts, Calendar, Tasks, Notes, and Journal folders.</span></span> <span data-ttu-id="c113c-121">Não existe forma de conceder acesso a itens privados apenas em pastas especificadas.</span><span class="sxs-lookup"><span data-stu-id="c113c-121">There is no way to grant access to private items in only specified folders.</span></span>

7. <span data-ttu-id="c113c-122">Selecione **OK**.</span><span class="sxs-lookup"><span data-stu-id="c113c-122">Choose **OK**.</span></span>

    > [!NOTE]
    >
    > - <span data-ttu-id="c113c-123">As mensagens enviadas com permissões enviar em nome incluem tanto as do delegado como os seus nomes ao lado **de From**.</span><span class="sxs-lookup"><span data-stu-id="c113c-123">Messages sent with Send on Behalf permissions include both the delegate's and your names next to **From**.</span></span> <span data-ttu-id="c113c-124">Quando uma mensagem é enviada com permissões de Envio como, apenas o seu nome aparece.</span><span class="sxs-lookup"><span data-stu-id="c113c-124">When a message is sent with Send As permissions, only your name appears.</span></span>
    > - <span data-ttu-id="c113c-125">Uma vez que adicione alguém como delegado, eles podem adicionar a sua caixa de correio Exchange ao seu perfil Outlook.</span><span class="sxs-lookup"><span data-stu-id="c113c-125">Once you add someone as a delegate, they can add your Exchange mailbox to their Outlook profile.</span></span> <span data-ttu-id="c113c-126">Para obter instruções, consulte [Gerir o correio e os itens de calendário de outra pessoa](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).</span><span class="sxs-lookup"><span data-stu-id="c113c-126">For instructions, see [Manage another person's mail and calendar items](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).</span></span>

<span data-ttu-id="c113c-127">Para remover um delegado no Outlook for Windows:</span><span class="sxs-lookup"><span data-stu-id="c113c-127">To remove a Delegate in Outlook for Windows:</span></span>

1. <span data-ttu-id="c113c-128">Clique no **separador Ficheiro.**</span><span class="sxs-lookup"><span data-stu-id="c113c-128">Click on the **File** tab.</span></span>
2. <span data-ttu-id="c113c-129">Clique em **Definições de Conta** seguida **de Acesso delegado.**</span><span class="sxs-lookup"><span data-stu-id="c113c-129">Click on **Account Settings** followed by **Delegate Access**.</span></span>
3. <span data-ttu-id="c113c-130">Escolha o nome do delegado para quem pretende alterar permissões e, em seguida, clique em **Remover** seguido por **OK**.</span><span class="sxs-lookup"><span data-stu-id="c113c-130">Choose the name of the delegate for whom you want to change permissions, and then click on **Remove** followed by **OK**.</span></span>
