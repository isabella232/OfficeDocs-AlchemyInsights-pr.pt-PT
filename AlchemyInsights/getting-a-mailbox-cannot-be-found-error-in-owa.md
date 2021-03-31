---
title: 126 A obtenção de uma caixa de correio não pode ser encontrada erro na OWA?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 6bab821aaa3b50c365ef5d25a61bca195c76d7ce
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426673"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a><span data-ttu-id="b87a0-102">Receber uma caixa de correio não encontrou erro no Outlook na web?</span><span class="sxs-lookup"><span data-stu-id="b87a0-102">Getting a mailbox not found error in Outlook on the web?</span></span>

<span data-ttu-id="b87a0-103">Se estiver a usar o Outlook na web e receber uma **Caixa de Correio não foi encontrada por** erro, a conta que usou para ligar ao Outlook na web não tem uma licença Exchange Online e, portanto, nenhuma caixa de correio está associada à conta.</span><span class="sxs-lookup"><span data-stu-id="b87a0-103">If you're using Outlook on the web and you get a **Mailbox couldn't be found for** error, the account that you used to connect to Outlook on the web doesn't have an Exchange Online license and therefore, no mailbox is associated with the account.</span></span> <span data-ttu-id="b87a0-104">O seu administrador pode atribuir uma licença à sua conta seguindo estes passos:</span><span class="sxs-lookup"><span data-stu-id="b87a0-104">Your admin can assign a license to your account by following these steps:</span></span>

1. <span data-ttu-id="b87a0-105">Abra o [centro de administração Microsoft 365](https://portal.office.com/adminportal/home#/homepage) e vá para **utilizadores Ativos** sob a secção **Utilizadores** e selecione o utilizador que está a ver o erro.</span><span class="sxs-lookup"><span data-stu-id="b87a0-105">Open the [Microsoft 365 admin center](https://portal.office.com/adminportal/home#/homepage) and go to **Active users** under the **Users** section, and select the user who is seeing the error.</span></span>

2. <span data-ttu-id="b87a0-106">Na página de utilizador que abre, aceda à secção **licenças e aplicações,** selecione o valor de **Localização** apropriado e atribua uma licença que contenha Exchange Online (expanda a licença para ver os seus dados).</span><span class="sxs-lookup"><span data-stu-id="b87a0-106">In the user page that opens, go to the **Licenses and Apps** section, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details).</span></span> <span data-ttu-id="b87a0-107">Quando terminar, clique em **Guardar as alterações.**</span><span class="sxs-lookup"><span data-stu-id="b87a0-107">When you're finished, click **Save changes**.</span></span>

<span data-ttu-id="b87a0-108">Em alguns casos, se a licença já estiver atribuída a uma conta de utilizador, remover e reatribuir a licença ajuda a resolver o problema e a obtê-la adequadamente a provisionada no sistema:</span><span class="sxs-lookup"><span data-stu-id="b87a0-108">In some cases, if the license is already assigned to a user account, removing and reassigning the license helps to resolve the issue and get it properly provisioned in the system:</span></span> 

- <span data-ttu-id="b87a0-109">Verifique se as suas subscrições M365 Exchange Online (e outras, caso tenha alguma) estão em vigor e não expiraram recentemente.</span><span class="sxs-lookup"><span data-stu-id="b87a0-109">Check to see if your M365 Exchange Online (and other, if you have any) subscriptions are current and have not recently expired.</span></span>

<span data-ttu-id="b87a0-110">Uma vez que tenha assegurado que a sua subscrição não expirou e que foi atribuída uma licença válida à conta de utilizador, pode demorar até 24 horas para que a licença seja antesetada, pelo que poderá ter de esperar que o seu problema seja resolvido.</span><span class="sxs-lookup"><span data-stu-id="b87a0-110">Once you have made sure that your subscription has not expired and a valid license has been assigned to the user account, it can take up to 24 hours for license to get provisioned, so you might have to wait for your issue to resolve.</span></span> <span data-ttu-id="b87a0-111">Para mais informações, consulte [Atribuir e gerir licenças.](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses)</span><span class="sxs-lookup"><span data-stu-id="b87a0-111">For more info, see [Assign and manage licenses](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses).</span></span>