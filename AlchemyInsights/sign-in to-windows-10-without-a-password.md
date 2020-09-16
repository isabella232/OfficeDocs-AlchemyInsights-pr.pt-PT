---
title: Iniciar s-in no Windows 10 sem utilizar uma senha
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 839b945c457cb007f13605c5b903ded75dadd1d7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47719964"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="df2f1-102">Iniciar s-in no Windows 10 sem utilizar uma senha</span><span class="sxs-lookup"><span data-stu-id="df2f1-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="df2f1-103">Para evitar ter de escrever uma palavra-passe no arranque do Windows, recomendamos que utilize uma das opções de entrada segura do Windows Hello, como um PIN, reconhecimento facial ou impressão digital, se disponível.</span><span class="sxs-lookup"><span data-stu-id="df2f1-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="df2f1-104">Se realmente pretender desativar o s-in seguro, consulte as instruções "Iniciar automaticamente o Windows 10" abaixo.</span><span class="sxs-lookup"><span data-stu-id="df2f1-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="df2f1-105">**Secure Windows Hello alternativas à senha de conta**</span><span class="sxs-lookup"><span data-stu-id="df2f1-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="df2f1-106">Aceda a **Definições > Contas > opções de inscrição** (ou clique [aqui).](ms-settings:signinoptions?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="df2f1-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="df2f1-107">As opções de inscrição disponíveis serão listadas.</span><span class="sxs-lookup"><span data-stu-id="df2f1-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="df2f1-108">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="df2f1-108">For example:</span></span>

![Opções de inscrição.](media/sign-in-options.png)

<span data-ttu-id="df2f1-110">Clique ou toque numa das opções para configurá-lo.</span><span class="sxs-lookup"><span data-stu-id="df2f1-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="df2f1-111">Da próxima vez que iniciar ou desbloquear o Windows, poderá utilizar a nova opção em vez de uma palavra-passe.</span><span class="sxs-lookup"><span data-stu-id="df2f1-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="df2f1-112">**Iniciar automaticamente o ó20.**</span><span class="sxs-lookup"><span data-stu-id="df2f1-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="df2f1-113">**Nota:** O acesso automático é conveniente, mas introduz um risco de segurança, especialmente se o seu PC estiver acessível por várias pessoas.</span><span class="sxs-lookup"><span data-stu-id="df2f1-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="df2f1-114">Clique ou toque no botão **Iniciar** na barra de tarefas.</span><span class="sxs-lookup"><span data-stu-id="df2f1-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="df2f1-115">Digite **netplwiz** e bata na tecla 'Introduzir' para abrir a janela Contas de Utilizador.</span><span class="sxs-lookup"><span data-stu-id="df2f1-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="df2f1-116">Nas **Contas de Utilizador,** clique na conta a que pretende iniciar automaticamente o seu início.</span><span class="sxs-lookup"><span data-stu-id="df2f1-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="df2f1-117">Desmarque a caixa de verificação "Os utilizadores devem introduzir um nome de utilizador e uma palavra-passe para utilizar este computador".</span><span class="sxs-lookup"><span data-stu-id="df2f1-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Os utilizadores devem introduzir uma opção de nome de utilizador e palavra-passe.](media/users-must-enter-username.png)

5. <span data-ttu-id="df2f1-119">Clique em **OK**.</span><span class="sxs-lookup"><span data-stu-id="df2f1-119">Click **OK**.</span></span> <span data-ttu-id="df2f1-120">Ser-lhe-á pedido que introduza e confirme a palavra-passe para a conta que selecionou.</span><span class="sxs-lookup"><span data-stu-id="df2f1-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="df2f1-121">Clique **em OK** para terminar.</span><span class="sxs-lookup"><span data-stu-id="df2f1-121">Click **OK** to finish.</span></span> <span data-ttu-id="df2f1-122">Da próxima vez que o Windows 10 começar, iniciará automaticamente o s registação na conta selecionada.</span><span class="sxs-lookup"><span data-stu-id="df2f1-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
