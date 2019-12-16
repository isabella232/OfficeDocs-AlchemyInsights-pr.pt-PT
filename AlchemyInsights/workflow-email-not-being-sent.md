---
title: E-mail de fluxo de trabalho não está sendo enviado
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: 76b64323c9d34d49e9c6bd77c2cc7eff6d7c5402
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049384"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="2097f-102">E-mail de fluxo de trabalho não está sendo enviado para uma lista ou biblioteca do SharePoint</span><span class="sxs-lookup"><span data-stu-id="2097f-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="2097f-103">Os e-mails dos fluxos de trabalho não são enviados para todos os usuários ou apenas usuários específicos, ou você vê o erro **A mensagem de e-mail não pode ser enviada. Certifique-se de que o e-mail tem um destinatário válido.**</span><span class="sxs-lookup"><span data-stu-id="2097f-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="2097f-104">Verifique se o usuário existe no grupo de permissões **de todas as pessoas** (lista de informações do usuário) para essa coleção do site.</span><span class="sxs-lookup"><span data-stu-id="2097f-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="2097f-105">Url direto da<tenant>amostra: https:// .sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId=0</span><span class="sxs-lookup"><span data-stu-id="2097f-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="2097f-106">Se o usuário não existir, certifique-se de que o usuário está inscrito na página.</span><span class="sxs-lookup"><span data-stu-id="2097f-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="2097f-107">Se for um usuário externo, certifique-se de que seu convite tenha sido aceito.</span><span class="sxs-lookup"><span data-stu-id="2097f-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="2097f-108">Se o usuário existir no grupo de permissões, certifique-se de que o endereço de e-mail esteja correto.</span><span class="sxs-lookup"><span data-stu-id="2097f-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="2097f-109">Se o endereço de e-mail dos usuários não for definido aqui, crie um alerta de amostra para aquele usuário que força a sincronização dessa conta de usuário, desde perfis de usuário do SharePoint até essa coleção do site.</span><span class="sxs-lookup"><span data-stu-id="2097f-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="2097f-110">E-mail de fluxos de trabalho são enviados para os administradores de coleta do site, mas não para outros usuários e ver o erro **HTTP Proibido para <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.sendemail**.</span><span class="sxs-lookup"><span data-stu-id="2097f-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="2097f-111">Veja o [Access Denied quando enviar um e-mail para um grupo SharePoint.](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups)</span><span class="sxs-lookup"><span data-stu-id="2097f-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="2097f-112">Além disso, verifique se o recurso de coleta do site de bloqueio de **permissão** de usuário de acesso limitado não está ativo.</span><span class="sxs-lookup"><span data-stu-id="2097f-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="2097f-113">Tópicos relacionados</span><span class="sxs-lookup"><span data-stu-id="2097f-113">Related topics</span></span>
<span data-ttu-id="2097f-114">Quer experimentar o Microsoft Flow no SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="2097f-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="2097f-115">Criar fluxo</span><span class="sxs-lookup"><span data-stu-id="2097f-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="2097f-116">SharePoint e Flow</span><span class="sxs-lookup"><span data-stu-id="2097f-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


