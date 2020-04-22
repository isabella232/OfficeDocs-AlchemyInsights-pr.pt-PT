---
title: Problemas de sessão em apps do Office
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
ms.openlocfilehash: 695d449a876c22ff441da2367ef67aaea470eb66
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43763012"
---
# <a name="issues-signing-in-to-office-apps"></a><span data-ttu-id="5ff37-102">Problemas de sessão em apps do Office</span><span class="sxs-lookup"><span data-stu-id="5ff37-102">Issues signing in to Office apps</span></span>

<span data-ttu-id="5ff37-103">Para corrigir problemas de inscrição com aplicações do Office, tente o seguinte:</span><span class="sxs-lookup"><span data-stu-id="5ff37-103">To fix sign-in issues with Office apps, try the following:</span></span>

- <span data-ttu-id="5ff37-104">Remova todas as contas de trabalho, exceto a conta afetada, utilizando as definições do Windows > **Trabalho de Acesso ou escola**.</span><span class="sxs-lookup"><span data-stu-id="5ff37-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="5ff37-105">[Credenciais de escritório claro](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) usando O Gestor Credencial do Windows.</span><span class="sxs-lookup"><span data-stu-id="5ff37-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="5ff37-106">**Nota:** As vias de registo do Office 2016 mudaram para 16,0.</span><span class="sxs-lookup"><span data-stu-id="5ff37-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="5ff37-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="5ff37-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="5ff37-108">Abra uma aplicação do Office, **escolha** > **Registo de Conta** > **Sign out**. Em seguida, inscreva-se utilizando uma conta de utilizador com uma licença válida.</span><span class="sxs-lookup"><span data-stu-id="5ff37-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="5ff37-109">Para obter informações detalhadas, consulte [Contas no Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="5ff37-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="5ff37-110">Para Mac, consulte [Não consigo iniciar sessão numa aplicação do Office 2016 para Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="5ff37-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>
- <span data-ttu-id="5ff37-111">Se os erros ocorrerem durante a ligação ao Microsoft 365 utilizando o Office 2013, ative a autenticação moderna para o cliente do Office.</span><span class="sxs-lookup"><span data-stu-id="5ff37-111">If the errors occurs while connecting to Microsoft 365 using Office 2013, enable modern authentication for Office client.</span></span>

<span data-ttu-id="5ff37-112">Para obter mais informações, consulte:</span><span class="sxs-lookup"><span data-stu-id="5ff37-112">For more information, see:</span></span>
- [<span data-ttu-id="5ff37-113">Não pode iniciar sessão na Microsoft 365, Azure ou Intune</span><span class="sxs-lookup"><span data-stu-id="5ff37-113">You can't sign in to Microsoft 365, Azure, or Intune</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [<span data-ttu-id="5ff37-114">Problemas de ligação no registo após atualização para o Office 2016 constroem 16.0.7967 no Windows 10</span><span class="sxs-lookup"><span data-stu-id="5ff37-114">Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10</span></span>](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- [<span data-ttu-id="5ff37-115">"Desculpe, outra conta da sua organização já está assinada neste computador" no Office</span><span class="sxs-lookup"><span data-stu-id="5ff37-115">"Sorry, another account from your organization is already signed in on this computer" in Office</span></span>](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [<span data-ttu-id="5ff37-116">Problemas de sessão de sessão com autenticação moderna do Office quando utiliza a ADFS</span><span class="sxs-lookup"><span data-stu-id="5ff37-116">Troubleshoot sign-in issues with Office modern authentication when you use ADFS</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)