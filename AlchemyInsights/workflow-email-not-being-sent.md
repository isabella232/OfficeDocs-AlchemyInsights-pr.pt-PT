---
title: O e-mail do workflow não está a ser enviado
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 391d3a2dcc2676a405065115f375c802d2492119
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766144"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="d3449-102">O e-mail workflow não está a ser enviado para uma lista de SharePoint ou biblioteca</span><span class="sxs-lookup"><span data-stu-id="d3449-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="d3449-103">O e-mail dos fluxos de trabalho não é enviado para todos os utilizadores ou apenas utilizadores específicos, ou vê o erro **A mensagem de correio eletrónico não pode ser enviada. Certifique-se de que o e-mail tem um destinatário válido**.</span><span class="sxs-lookup"><span data-stu-id="d3449-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="d3449-104">Verifique se o utilizador existe no grupo de permissões **All People** (lista de informações do utilizador) para essa recolha do site.</span><span class="sxs-lookup"><span data-stu-id="d3449-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="d3449-105">URL direto da<tenant>amostra: https:// .sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId=0</span><span class="sxs-lookup"><span data-stu-id="d3449-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="d3449-106">Se o utilizador não existir, certifique-se de que o utilizador está inscrito na página.</span><span class="sxs-lookup"><span data-stu-id="d3449-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="d3449-107">Se for um utilizador externo, certifique-se de que o seu convite foi aceite.</span><span class="sxs-lookup"><span data-stu-id="d3449-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="d3449-108">Se o utilizador existir no grupo de permissões, certifique-se de que o endereço de e-mail está correto.</span><span class="sxs-lookup"><span data-stu-id="d3449-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="d3449-109">Se o endereço de e-mail dos utilizadores não estiver definido aqui, crie um alerta de amostra para esse utilizador que força a sincronização dessa conta de utilizador desde os Perfis de Utilizador do SharePoint até à recolha do site.</span><span class="sxs-lookup"><span data-stu-id="d3449-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="d3449-110">O e-mail dos fluxos de trabalho é enviado aos administradores de recolha do site, mas não a outros utilizadores e ver o erro **HTTP Proibido de <span>https:</span>//URL/_vti_bin/cliente.xvc.sp.utilities.utility.sendEmail**.</span><span class="sxs-lookup"><span data-stu-id="d3449-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="d3449-111">Ver [Acesso Negado quando envia um e-mail para um grupo SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="d3449-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="d3449-112">Além disso, verifique se a funcionalidade de recolha do modo de **bloqueio de autorização do utilizador** de acesso limitado não está ativa.</span><span class="sxs-lookup"><span data-stu-id="d3449-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="d3449-113">Tópicos relacionados</span><span class="sxs-lookup"><span data-stu-id="d3449-113">Related topics</span></span>
<span data-ttu-id="d3449-114">Quer experimentar o Microsoft Flow no SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="d3449-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="d3449-115">Criar fluxo</span><span class="sxs-lookup"><span data-stu-id="d3449-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="d3449-116">SharePoint e Flow</span><span class="sxs-lookup"><span data-stu-id="d3449-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


