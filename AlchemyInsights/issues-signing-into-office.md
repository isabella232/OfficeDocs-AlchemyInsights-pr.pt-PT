---
title: Problemas de início de sessão em aplicações do Office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2574"
ms.openlocfilehash: 3622a3408b25b43090e9414ae5ffcfc2760264ee
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938302"
---
# <a name="issues-signing-in-to-office-apps"></a><span data-ttu-id="a648a-102">Problemas de início de sessão em aplicações do Office</span><span class="sxs-lookup"><span data-stu-id="a648a-102">Issues signing in to Office apps</span></span>

<span data-ttu-id="a648a-103">Para corrigir problemas de início de sessão com aplicações do Office, tente o seguinte:</span><span class="sxs-lookup"><span data-stu-id="a648a-103">To fix sign-in issues with Office apps, try the following:</span></span>

- <span data-ttu-id="a648a-104">Remova todas as contas de trabalho, excepto a conta afectada, utilizando as definições do Windows > **trabalho do Access ou na escola**.</span><span class="sxs-lookup"><span data-stu-id="a648a-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="a648a-105">[Office Limpar credenciais](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) utilizando o Gestor de credenciais do Windows.</span><span class="sxs-lookup"><span data-stu-id="a648a-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="a648a-106">**Nota:** Os caminhos de registo para o Office 2016 foram alterados para 16,0.</span><span class="sxs-lookup"><span data-stu-id="a648a-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="a648a-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="a648a-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="a648a-108">Abra uma aplicação do Office, seleccione o **ficheiro** > **conta** > **Terminar sessão**. Em seguida, inicie sessão utilizando uma conta de utilizador com uma licença válida.</span><span class="sxs-lookup"><span data-stu-id="a648a-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="a648a-109">Para obter informações detalhadas, consulte [contas no Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="a648a-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="a648a-110">Para Mac, consulte a ' [não é possível iniciar sessão num 2016 do Office para Mac Apl](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="a648a-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>
- <span data-ttu-id="a648a-111">Se ocorrer erros ao estabelecer a ligação utilizando o Office 2013 do Office 365, Active a autenticação moderna de cliente do Office.</span><span class="sxs-lookup"><span data-stu-id="a648a-111">If the errors occurs while connecting to Office 365 using Office 2013, enable modern authentication for Office client.</span></span>

<span data-ttu-id="a648a-112">Para obter mais informações, consulte:</span><span class="sxs-lookup"><span data-stu-id="a648a-112">For more information, see:</span></span>
- [<span data-ttu-id="a648a-113">É possível iniciar sessão Office 365, Azure ou Intune</span><span class="sxs-lookup"><span data-stu-id="a648a-113">You can't sign in to Office 365, Azure, or Intune</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [<span data-ttu-id="a648a-114">Problemas de ligação no início de sessão-in após a actualização do Office de 2016 compilação 16.0.7967 no Windows 10</span><span class="sxs-lookup"><span data-stu-id="a648a-114">Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10</span></span>](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- [<span data-ttu-id="a648a-115">"Pedido de desculpa, outra conta da sua organização é ainda tiver sessão iniciada neste computador" no Office</span><span class="sxs-lookup"><span data-stu-id="a648a-115">"Sorry, another account from your organization is already signed in on this computer" in Office</span></span>](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [<span data-ttu-id="a648a-116">Resolução de problemas de início de sessão com autenticação moderna do Office quando utiliza o ADFS</span><span class="sxs-lookup"><span data-stu-id="a648a-116">Troubleshoot sign-in issues with Office modern authentication when you use ADFS</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)