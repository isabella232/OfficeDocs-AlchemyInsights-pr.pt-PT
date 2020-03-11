---
title: Iniciar sessão no Windows 10 sem usar uma senha
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 1f325eb7afb1e88457296e8187f8ba6dff2ebfe0
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588291"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="7ec25-102">Iniciar sessão no Windows 10 sem usar uma senha</span><span class="sxs-lookup"><span data-stu-id="7ec25-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="7ec25-103">Para evitar ter de escrever uma palavra-passe no arranque do Windows, recomendamos que utilize uma das opções de entrada segura do Windows Hello, como um PIN, reconhecimento facial ou impressão digital, se disponível.</span><span class="sxs-lookup"><span data-stu-id="7ec25-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="7ec25-104">Se realmente quiser desativar o acesso seguro, consulte as instruções "Iniciar automaticamente o sessão no Windows 10" abaixo.</span><span class="sxs-lookup"><span data-stu-id="7ec25-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="7ec25-105">**Alternativas Secure Windows Hello à palavra-passe da conta**</span><span class="sxs-lookup"><span data-stu-id="7ec25-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="7ec25-106">Vá a **Definições > Contas > opções de iniciar sessão** (ou clique [aqui](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="7ec25-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="7ec25-107">As opções de inscrição disponíveis serão listadas.</span><span class="sxs-lookup"><span data-stu-id="7ec25-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="7ec25-108">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="7ec25-108">For example:</span></span>

![Opções de inscrição.](media/sign-in-options.png)

<span data-ttu-id="7ec25-110">Clique ou toque numa das opções para configurá-lo.</span><span class="sxs-lookup"><span data-stu-id="7ec25-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="7ec25-111">Da próxima vez que iniciar ou desbloquear o Windows, poderá utilizar a nova opção em vez de uma palavra-passe.</span><span class="sxs-lookup"><span data-stu-id="7ec25-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="7ec25-112">**Iniciar sessão automática no Windows 10**</span><span class="sxs-lookup"><span data-stu-id="7ec25-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="7ec25-113">**Nota:** O início automático é conveniente, mas introduz um risco de segurança, especialmente se o seu PC estiver acessível por várias pessoas.</span><span class="sxs-lookup"><span data-stu-id="7ec25-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="7ec25-114">Clique ou toque no botão **Iniciar** na barra de tarefas.</span><span class="sxs-lookup"><span data-stu-id="7ec25-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="7ec25-115">Digite **netplwiz** e acerte na tecla Enter para abrir a janela contas do utilizador.</span><span class="sxs-lookup"><span data-stu-id="7ec25-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="7ec25-116">Nas **Contas do Utilizador,** clique na conta para a sua assinatura automaticamente quando o Windows começar.</span><span class="sxs-lookup"><span data-stu-id="7ec25-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="7ec25-117">Desmarque a caixa de verificação "Os utilizadores devem introduzir um nome de utilizador e uma senha para utilizar este computador".</span><span class="sxs-lookup"><span data-stu-id="7ec25-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Os utilizadores devem introduzir uma opção de username e password.](media/users-must-enter-username.png)

5. <span data-ttu-id="7ec25-119">Clique em **OK**.</span><span class="sxs-lookup"><span data-stu-id="7ec25-119">Click **OK**.</span></span> <span data-ttu-id="7ec25-120">Será-lhe pedido que introduza e confirme a palavra-passe para a conta selecionada.</span><span class="sxs-lookup"><span data-stu-id="7ec25-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="7ec25-121">Clique **em OK** para terminar.</span><span class="sxs-lookup"><span data-stu-id="7ec25-121">Click **OK** to finish.</span></span> <span data-ttu-id="7ec25-122">Da próxima vez que o Windows 10 começar, iniciará automaticamente o seu início na conta selecionada.</span><span class="sxs-lookup"><span data-stu-id="7ec25-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
