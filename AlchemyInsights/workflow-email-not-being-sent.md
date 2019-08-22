---
title: Não está a ser enviado correio electrónico de fluxo de trabalho
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 261fe1b1bc815dd4ad568051cfefad1e214b957e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36530896"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="dc690-102">Correio electrónico de fluxo de trabalho não está a ser enviado para uma lista do SharePoint ou biblioteca</span><span class="sxs-lookup"><span data-stu-id="dc690-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="dc690-103">Mensagem de correio electrónico fluxos de trabalho não são enviadas para todos os utilizadores ou apenas utilizadores específicos ou ver que o erro **a mensagem de correio electrónico não pode ser enviado. Certifique-se o correio electrónico tem um destinatário válido**.</span><span class="sxs-lookup"><span data-stu-id="dc690-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="dc690-104">Verifique se o utilizador existir no grupo de permissões de **Todas as pessoas** (lista de informações de utilizador) para essa colecção de sites.</span><span class="sxs-lookup"><span data-stu-id="dc690-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="dc690-105">Exemplo de URL directa: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="dc690-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="dc690-106">Se o utilizador não existir, certifique-se do que utilizador inicia sessão na página.</span><span class="sxs-lookup"><span data-stu-id="dc690-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="dc690-107">Se for um utilizador externo, certifique-se de que o seu convite foi aceite.</span><span class="sxs-lookup"><span data-stu-id="dc690-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="dc690-108">Se o utilizador existir no grupo de permissões, certificar-se de que o endereço de correio electrónico está correcto.</span><span class="sxs-lookup"><span data-stu-id="dc690-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="dc690-109">Se o endereço de correio electrónico de utilizadores não estiver definido aqui, em seguida, crie um alerta de exemplo para esse utilizador que obriga a sincronização dessa conta de utilizador de perfis de utilizador do SharePoint para esta colecção de sites.</span><span class="sxs-lookup"><span data-stu-id="dc690-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="dc690-110">Mensagem de correio electrónico fluxos de trabalho são enviados para os administradores de colecção de sites, mas não para outros utilizadores e ver o erro **HTTP proibido a <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span><span class="sxs-lookup"><span data-stu-id="dc690-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="dc690-111">Consulte [o acesso negado quando envia uma mensagem de correio electrónico a um grupo SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="dc690-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="dc690-112">Além disso, certifique-se de que a funcionalidade de colecção de sites de **modo de bloqueio de permissão de utilizador de acesso limitado** não está activa.</span><span class="sxs-lookup"><span data-stu-id="dc690-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="dc690-113">Tópicos relacionados</span><span class="sxs-lookup"><span data-stu-id="dc690-113">Related topics</span></span>
<span data-ttu-id="dc690-114">Pretende tentar Microsoft Flow no SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="dc690-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="dc690-115">Criar fluxo</span><span class="sxs-lookup"><span data-stu-id="dc690-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="dc690-116">Fluxo e do SharePoint</span><span class="sxs-lookup"><span data-stu-id="dc690-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


