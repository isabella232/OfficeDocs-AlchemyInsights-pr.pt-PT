---
title: Definir respostas automáticas numa caixa de correio
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: aeeb2e1e76fe602d2767b422797452fd1155fdd5
ms.sourcegitcommit: fdfd41c2bfb2d45003b3906e6469377384a91cb5
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2020
ms.locfileid: "43509512"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a><span data-ttu-id="a6b6f-102">Definir respostas automáticas na caixa de correio de um utilizador</span><span class="sxs-lookup"><span data-stu-id="a6b6f-102">Set auto replies for a user's mailbox</span></span>

<span data-ttu-id="a6b6f-103">**Método 1**</span><span class="sxs-lookup"><span data-stu-id="a6b6f-103">**Method 1**</span></span>

1. <span data-ttu-id="a6b6f-104">Inicie sessão no portal do Office 365.</span><span class="sxs-lookup"><span data-stu-id="a6b6f-104">Sign in to the Office 365 portal.</span></span>

2. <span data-ttu-id="a6b6f-105">Aceda a **Utilizadores > Utilizadores ativos** (ou **Grupos > Caixas de correio partilhadas** se a definição for implementada numa caixa de correio partilhada).</span><span class="sxs-lookup"><span data-stu-id="a6b6f-105">Go to **Users > Active users** (or **Groups > Shared mailboxes** if you set this on a shared mailbox).</span></span>

3. <span data-ttu-id="a6b6f-106">Selecione um utilizador que tenha uma caixa de correio do Microsoft Exchange.</span><span class="sxs-lookup"><span data-stu-id="a6b6f-106">Select a user who has a Microsoft Exchange mailbox.</span></span>

4. <span data-ttu-id="a6b6f-107">No menu de contexto à direita, aceda a **Definições de correio > Respostas automáticas** (se for uma caixa de correio partilhada, basta clicar em **Respostas automáticas** no menu de contexto).</span><span class="sxs-lookup"><span data-stu-id="a6b6f-107">On the fly-out menu on the right, go to **Mail settings > Automatic replies** (if it's a shared mailbox, just click **Automatic replies** on the fly-out).</span></span>

<span data-ttu-id="a6b6f-108">**Método 2**</span><span class="sxs-lookup"><span data-stu-id="a6b6f-108">**Method 2**</span></span>

1. <span data-ttu-id="a6b6f-109">Inicie sessão no portal de administração do Office 365 com credenciais de administrador.</span><span class="sxs-lookup"><span data-stu-id="a6b6f-109">Sign in to the Office 365 admin portal by using administrator credentials.</span></span>

2. <span data-ttu-id="a6b6f-110">Expanda **Centros de Administração** e, em seguida, clique em **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="a6b6f-110">Expand **Admin Centers**, and then click **Exchange**.</span></span>

3. <span data-ttu-id="a6b6f-111">Clique na imagem no canto superior direito, clique em **Outro Utilizador** e, em seguida, selecione a caixa de correio do utilizador que pretende alterar.</span><span class="sxs-lookup"><span data-stu-id="a6b6f-111">Click the picture in the upper-right corner, click **Another User**, and then select the user mailbox that you want to change.</span></span>

4. <span data-ttu-id="a6b6f-112">No lado esquerdo, selecione **Opções**, clique em **Organizar E-mail** e clique em **Respostas automáticas.**</span><span class="sxs-lookup"><span data-stu-id="a6b6f-112">On the left side, select **Options**, click **Organize E-mail**, and then click **Automatic replies.**</span></span>

<span data-ttu-id="a6b6f-113">**Método 3**</span><span class="sxs-lookup"><span data-stu-id="a6b6f-113">**Method 3**</span></span>

<span data-ttu-id="a6b6f-114">Execute o seguinte cmdlet no PowerShell do Exchange Online:</span><span class="sxs-lookup"><span data-stu-id="a6b6f-114">Run the following cmdlet in Exchange Online PowerShell:</span></span>

<span data-ttu-id="a6b6f-115">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="a6b6f-115">PowerShellCopy</span></span>

```
    Set-MailboxAutoReplyConfiguration
```

<span data-ttu-id="a6b6f-116">Para mais informações acerca deste cmdlet, consulte [Configurar MailboxAutoAnswerConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span><span class="sxs-lookup"><span data-stu-id="a6b6f-116">For more information about this cmdlet, see [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span></span>
