---
title: Utilizador recebe erro AADSTS7000112 Yammer está desativado
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: c92b09ee9a9ca06f85906e7fce601582a7e83244
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198375"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a><span data-ttu-id="1ead2-102">Utilizador recebe erro AADSTS7000112 Yammer está desativado</span><span class="sxs-lookup"><span data-stu-id="1ead2-102">User receives error AADSTS7000112 Yammer is disabled</span></span>

<span data-ttu-id="1ead2-103">Se receber o erro "AADSTS7000112: Aplicação '0000005-0000-0ff1-ce00-0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000-000-0ff1-0000000000000000000000000000000</span><span class="sxs-lookup"><span data-stu-id="1ead2-103">If you receive the error "AADSTS7000112: Application '00000005-0000-0ff1-ce00-000000000000'(Yammer) is disabled", a problem exists with the service principal within Azure AD.</span></span> <span data-ttu-id="1ead2-104">Um administrador pode ter desativado o diretor de serviço para bloquear o acesso ao Yammer.</span><span class="sxs-lookup"><span data-stu-id="1ead2-104">An administrator might have disabled the service principal to block access to Yammer.</span></span>

<span data-ttu-id="1ead2-105">A desativação do diretor de serviço não é recomendada e pode causar problemas adicionais.</span><span class="sxs-lookup"><span data-stu-id="1ead2-105">Disabling the service principal is not recommended and can cause additional issues.</span></span> <span data-ttu-id="1ead2-106">Para obter mais informações sobre a abordagem suportada para bloquear o acesso do utilizador ao Yammer, consulte [Desligue o acesso do Yammer aos utilizadores da Microsoft 365](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span><span class="sxs-lookup"><span data-stu-id="1ead2-106">For more info about the supported approach to block user access to Yammer, see [Turn off Yammer access for Microsoft 365 users](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span></span>  

<span data-ttu-id="1ead2-107">Para corrigir este problema no Portal Azure e restaurar o acesso do utilizador ao Yammer:</span><span class="sxs-lookup"><span data-stu-id="1ead2-107">To correct this issue in the Azure Portal and restore user access to Yammer:</span></span>

1.  <span data-ttu-id="1ead2-108">Abra a página do Diretório Ativo Azure e selecione **aplicações Enterprise** em **Manage** no painel de navegação esquerdo.</span><span class="sxs-lookup"><span data-stu-id="1ead2-108">Open the Azure Active Directory page, and select **Enterprise applications** under **Manage** in the left navigation pane.</span></span>
3.  <span data-ttu-id="1ead2-109">Digite **Office 365 Yammer** na caixa de pesquisa e selecione o nome da aplicação para abrir as definições.</span><span class="sxs-lookup"><span data-stu-id="1ead2-109">Type **Office 365 Yammer** in the search box, and select the application name to open settings.</span></span>
4.  <span data-ttu-id="1ead2-110">Selecione **Propriedades** em **Manage** no painel de navegação esquerdo.</span><span class="sxs-lookup"><span data-stu-id="1ead2-110">Select **Properties** under **Manage** in the left navigation pane.</span></span>
5.  <span data-ttu-id="1ead2-111">Descreva o valor do **Yes** **Enabled para que os utilizadores se inscrevam?** **Save**</span><span class="sxs-lookup"><span data-stu-id="1ead2-111">Set the value of **Enabled for users to sign-in?** to **Yes**, and then select **Save**.</span></span>
6.  <span data-ttu-id="1ead2-112">Inscreva-se no Yammer de novo.</span><span class="sxs-lookup"><span data-stu-id="1ead2-112">Sign in to Yammer again.</span></span> <span data-ttu-id="1ead2-113">Talvez precise de limpar os biscoitos.</span><span class="sxs-lookup"><span data-stu-id="1ead2-113">You might need to clear cookies.</span></span>

<span data-ttu-id="1ead2-114">Em alternativa, executar comandos PowerShell para definir o valor.</span><span class="sxs-lookup"><span data-stu-id="1ead2-114">Alternatively, run PowerShell commands to set the value.</span></span> <span data-ttu-id="1ead2-115">Para mais informações, consulte ["Desculpe, mas estamos com dificuldades em inscrevê-lo" quando clicar no azulejo Yammer no Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="1ead2-115">For more info, see ["Sorry, but we're having trouble signing you in" error when you click the Yammer tile in Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span></span> 