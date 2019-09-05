---
title: Adicionar utilizadores externos a um grupo de distribuição
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: e84a5b04d6fc805deaa47cb10c91081f37411e5b
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/04/2019
ms.locfileid: "36737884"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="51f83-102">Adicionar utilizadores externos a um grupo de distribuição</span><span class="sxs-lookup"><span data-stu-id="51f83-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="51f83-103">Adicionar um contacto externo para um grupo de distribuição (DG) é um processo composto por dois passos:</span><span class="sxs-lookup"><span data-stu-id="51f83-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="51f83-104">Crie um contacto de correio para o utilizador externo:</span><span class="sxs-lookup"><span data-stu-id="51f83-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="51f83-105">No Centro de administração, vá para os **utilizadores** > página de[contactos](https://admin.microsoft.com/adminportal/home#/Contact) .</span><span class="sxs-lookup"><span data-stu-id="51f83-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="51f83-106">Seleccione **Adicionar um contacto**.</span><span class="sxs-lookup"><span data-stu-id="51f83-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="51f83-107">Escreva as informações para contacto e seleccione **Adicionar**.</span><span class="sxs-lookup"><span data-stu-id="51f83-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="51f83-108">Adicione o contacto de correio para a direcção-geral:</span><span class="sxs-lookup"><span data-stu-id="51f83-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="51f83-109">No Centro de administração, vá para os **grupos** > página[grupos](https://admin.microsoft.com/adminportal/home#/groups) .</span><span class="sxs-lookup"><span data-stu-id="51f83-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="51f83-110">Localizar DG que pretende adicionar o utilizador externo e, seleccione-a para abrir a caixa de diálogo de edição.</span><span class="sxs-lookup"><span data-stu-id="51f83-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="51f83-111">No separador **Membros** , seleccione **Ver tudo e gerir os membros**.</span><span class="sxs-lookup"><span data-stu-id="51f83-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="51f83-112">Seleccione **Adicionar membros**.</span><span class="sxs-lookup"><span data-stu-id="51f83-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="51f83-113">Seleccione o contacto de correio que criou no passo anterior e, em seguida, seleccione **Guardar**.</span><span class="sxs-lookup"><span data-stu-id="51f83-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="51f83-114">Se depois de seguir estes passos utilizadores externos não é possível enviar mensagens de correio electrónico para a direcção-geral ou se não recebem mensagens de correio electrónico a partir do mesmo, é possível que a direcção-geral está marcada para permitir apenas mensagens de correio electrónico de utilizadores internos.</span><span class="sxs-lookup"><span data-stu-id="51f83-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="51f83-115">Pode verificar esta configuração e corrigi-lo seguindo as instruções [aqui](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span><span class="sxs-lookup"><span data-stu-id="51f83-115">You can check this configuration and fix it following the directions [here](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span></span>
  
 <span data-ttu-id="51f83-116">**Nota:** Estas instruções não se aplicam se o tipo de um grupo é "Grupo do Office 365" em vez de "Grupo de distribuição".</span><span class="sxs-lookup"><span data-stu-id="51f83-116">**Note:** These instructions don't apply if your group's type is "Office 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="51f83-117">Se for esse o caso, pode adicionar o utilizador externo directamente para o grupo a partir do Outlook.</span><span class="sxs-lookup"><span data-stu-id="51f83-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="51f83-118">Obter informações detalhadas sobre os convidados de grupos do Office 365, bem como instruções para adicionar convidados externos podem encontrar-se no [presente artigo](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span><span class="sxs-lookup"><span data-stu-id="51f83-118">Detailed information on Office 365 groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  