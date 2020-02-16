---
title: Fixação das Aplicações do Office A sua conta está numa mensagem de mau estado
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: e591c56dd207a5bcb3979be3f66052121100b162
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/27/2019
ms.locfileid: "41969693"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a><span data-ttu-id="7e663-102">Corrigir as aplicações do Office "A sua conta está em mau estado" erro</span><span class="sxs-lookup"><span data-stu-id="7e663-102">Fixing the Office apps "Your account is in a bad state" error</span></span>

<span data-ttu-id="7e663-103">Para corrigir este erro, tente as seguintes opções no computador afetado:</span><span class="sxs-lookup"><span data-stu-id="7e663-103">To fix this error, try the following options on the affected computer:</span></span>

- <span data-ttu-id="7e663-104">Abra uma aplicação do Office, selecione **File** > **Account** > Sign out de todas as**contas**.</span><span class="sxs-lookup"><span data-stu-id="7e663-104">Open an Office app, select **File** > **Account** > **Sign Out of all accounts**.</span></span> <span data-ttu-id="7e663-105">Volte a fazer o sessão utilizando uma conta de utilizador com uma licença válida.</span><span class="sxs-lookup"><span data-stu-id="7e663-105">Sign in again using a user account with a valid license.</span></span> <span data-ttu-id="7e663-106">Para obter informações [detalhadas,](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9)consulte contas no Office .</span><span class="sxs-lookup"><span data-stu-id="7e663-106">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="7e663-107">[Credenciais de escritório claro](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) usando O Gestor Credencial do Windows.</span><span class="sxs-lookup"><span data-stu-id="7e663-107">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br>
  <span data-ttu-id="7e663-108">**Nota:** As vias de registo do Office 2016 mudaram para 16,0.</span><span class="sxs-lookup"><span data-stu-id="7e663-108">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="7e663-109">Por exemplo, \Software\Microsoft\Office\16.0\Common\Identity</span><span class="sxs-lookup"><span data-stu-id="7e663-109">For example, \Software\Microsoft\Office\16.0\Common\Identity</span></span>\
- <span data-ttu-id="7e663-110">No computador afetado, coloque o EnableADAL = 0 utilizando os seguintes passos:</span><span class="sxs-lookup"><span data-stu-id="7e663-110">On the affected computer, set the EnableADAL = 0 using the following steps:</span></span>  
     1. <span data-ttu-id="7e663-111">Clique no botão Windows e selecione **Executar**.</span><span class="sxs-lookup"><span data-stu-id="7e663-111">Right-click the Windows button and select **Run**.</span></span> <span data-ttu-id="7e663-112">Na caixa **Aberta,** escreva **regedite,** e, em seguida, selecione **OK**.</span><span class="sxs-lookup"><span data-stu-id="7e663-112">In the **Open** box, type **regedit**, and then select **OK**.</span></span>
     2. <span data-ttu-id="7e663-113">Selecione **Sim** quando solicitado para permitir que o Editor de Registo faça alterações no seu dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7e663-113">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="7e663-114">No Editor de Registo, adicione um valor DWORD de EnableADAL com uma definição de 0 em HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="7e663-114">In the Registry Editor, add a DWORD value of EnableADAL with a setting of 0 under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>
- <span data-ttu-id="7e663-115">Se o erro ocorrer durante a ligação ao Office 365 utilizando o Office 2013, ative a [autenticação moderna](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) para o cliente do Office.</span><span class="sxs-lookup"><span data-stu-id="7e663-115">If the error occurs while connecting to Office 365 using Office 2013, [enable modern authentication](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) for the Office client.</span></span>

<span data-ttu-id="7e663-116">Para mais informações, consulte [Como resolver aplicações não-navegadoras que não podem iniciar sessão no Office 365, Azure ou Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span><span class="sxs-lookup"><span data-stu-id="7e663-116">For more information, see [How to troubleshoot non-browser apps that can't sign in to Office 365, Azure, or Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span></span>

