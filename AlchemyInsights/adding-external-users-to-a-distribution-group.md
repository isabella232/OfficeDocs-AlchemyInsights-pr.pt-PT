---
title: Adicionar utilizadores externos a um Grupo de Distribuição
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 03cfd2c576cb03cbefd524a4ab6f04e2ef1eebec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663524"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="4692a-102">Adicionar utilizadores externos a um Grupo de Distribuição</span><span class="sxs-lookup"><span data-stu-id="4692a-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="4692a-103">A adição de um contacto externo a um Grupo de Distribuição (DG) é um processo em duas fases:</span><span class="sxs-lookup"><span data-stu-id="4692a-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="4692a-104">Criar um Contacto de Correio para o utilizador externo:</span><span class="sxs-lookup"><span data-stu-id="4692a-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="4692a-105">No centro de administração, aceda à página **Contactos dos Utilizadores.**  >  [Contacts](https://admin.microsoft.com/adminportal/home#/Contact)</span><span class="sxs-lookup"><span data-stu-id="4692a-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="4692a-106">**Selecione Adicione um contacto**.</span><span class="sxs-lookup"><span data-stu-id="4692a-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="4692a-107">Digite as informações para o seu contacto e selecione **Adicionar**.</span><span class="sxs-lookup"><span data-stu-id="4692a-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="4692a-108">Adicione o Contacto de Correio à sua DG:</span><span class="sxs-lookup"><span data-stu-id="4692a-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="4692a-109">No centro de administração, **Groups**aceda à página  >  [grupos de grupos.](https://admin.microsoft.com/adminportal/home#/groups)</span><span class="sxs-lookup"><span data-stu-id="4692a-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="4692a-110">Encontre a DG a que pretende adicionar o utilizador externo e selecione-o para abrir o diálogo de edição.</span><span class="sxs-lookup"><span data-stu-id="4692a-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="4692a-111">No separador **Membros,** **selecione Ver todos e gerir os membros**.</span><span class="sxs-lookup"><span data-stu-id="4692a-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="4692a-112">Selecione **Adicionar os membros**.</span><span class="sxs-lookup"><span data-stu-id="4692a-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="4692a-113">Selecione o Contacto de Correio que criou no passo anterior e, em seguida, **selecione Guardar**.</span><span class="sxs-lookup"><span data-stu-id="4692a-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="4692a-114">Se depois de seguir estes passos os seus utilizadores externos não puderem enviar e-mails à DG ou não receberem e-mails do mesmo, pode ser que a DG esteja marcada apenas para permitir e-mails de utilizadores internos.</span><span class="sxs-lookup"><span data-stu-id="4692a-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="4692a-115">Pode verificar esta configuração e corrigi-la seguindo as instruções [aqui](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span><span class="sxs-lookup"><span data-stu-id="4692a-115">You can check this configuration and fix it following the directions [here](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span></span>
  
 <span data-ttu-id="4692a-116">**Nota:** Estas instruções não se aplicam se o tipo do seu grupo for "Microsoft 365 group" em vez de "Grupo de Distribuição".</span><span class="sxs-lookup"><span data-stu-id="4692a-116">**Note:** These instructions don't apply if your group's type is "Microsoft 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="4692a-117">Se for esse o caso, pode adicionar o utilizador externo diretamente ao grupo do Outlook.</span><span class="sxs-lookup"><span data-stu-id="4692a-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="4692a-118">Informações detalhadas sobre os hóspedes do Grupo Microsoft 365, bem como instruções para a adição de hóspedes externos podem ser encontradas [neste artigo.](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)</span><span class="sxs-lookup"><span data-stu-id="4692a-118">Detailed information on Microsoft 365 Groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  