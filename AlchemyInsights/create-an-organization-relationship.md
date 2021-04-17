---
title: Criar uma Relação da Organização para permitir que os seus utilizadores colaborem com outra organização
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: b595fb87e18a055a7df1ff4c782a93591dd1f024
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816139"
---
# <a name="create-an-organization-relationship-to-allow-your-users-to-collaborate-with-another-organization"></a><span data-ttu-id="b5f3d-102">Criar uma Relação da Organização para permitir que os seus utilizadores colaborem com outra organização</span><span class="sxs-lookup"><span data-stu-id="b5f3d-102">Create an Organization Relationship to allow your users to collaborate with another organization</span></span>

1. <span data-ttu-id="b5f3d-103">A partir do dashboard do centro de administração do Microsoft 365, aceda a **Admin** > **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="b5f3d-103">From the Microsoft 365 admin center dashboard, go to **Admin** > **Exchange**.</span></span>
2. <span data-ttu-id="b5f3d-104">Aceda a **organização** > **partilha**.</span><span class="sxs-lookup"><span data-stu-id="b5f3d-104">Go to **organization** > **sharing**.</span></span>
3. <span data-ttu-id="b5f3d-105">Em **Partilha de Organização**, clique em **Nova** .</span><span class="sxs-lookup"><span data-stu-id="b5f3d-105">Under **Organization Sharing**, click **New** .</span></span>
4. <span data-ttu-id="b5f3d-106">Na **nova relação da organização**, na caixa **nome da Relação**, escreva um nome amigável para a relação da organização.</span><span class="sxs-lookup"><span data-stu-id="b5f3d-106">In **new organization relationship**, in the **Relationship name** box, type a friendly name for the organization relationship.</span></span>
5. <span data-ttu-id="b5f3d-107">Na caixa **Domínios para partilhar**, escreva o domínio para a organização externa do Office 365 ou do Exchange no local que pretende ver os seus calendários.</span><span class="sxs-lookup"><span data-stu-id="b5f3d-107">In the **Domains to share with** box, type the domain for the external Office 365 or Exchange on-premises organization you want to let see your calendars.</span></span> <span data-ttu-id="b5f3d-108">Se precisar de introduzir mais do que um domínio, separe os nomes de domínio com uma vírgula.</span><span class="sxs-lookup"><span data-stu-id="b5f3d-108">If you need to enter more than one domain, separate the domain names with a comma.</span></span> <span data-ttu-id="b5f3d-109">Por exemplo, contoso.com, service.contoso.com.</span><span class="sxs-lookup"><span data-stu-id="b5f3d-109">For example, contoso.com, service.contoso.com.</span></span>
6. <span data-ttu-id="b5f3d-110">Selecione a caixa de verificação **Ativar a partilha de informações de disponibilidade do calendário** para ativar a partilha de calendários com os domínios listados.</span><span class="sxs-lookup"><span data-stu-id="b5f3d-110">Select the **Enable calendar free/busy information sharing** check box to turn on calendar sharing with the domains you listed.</span></span> <span data-ttu-id="b5f3d-111">Defina o nível de partilha das informações de disponibilidade do calendário e defina os utilizadores que podem partilhar informações de disponibilidade do calendário.</span><span class="sxs-lookup"><span data-stu-id="b5f3d-111">Set the sharing level for calendar free/busy information and set which users can share calendar free/busy information.</span></span>  

<span data-ttu-id="b5f3d-112">Para definir o nível de acesso de disponibilidade, selecione uma das seguintes opções:</span><span class="sxs-lookup"><span data-stu-id="b5f3d-112">To set the free/busy access level, select one of the following:</span></span>

- <span data-ttu-id="b5f3d-113">**Informações de disponibilidade do calendário apenas com as horas**</span><span class="sxs-lookup"><span data-stu-id="b5f3d-113">**Calendar free/busy information with time only**</span></span>
- <span data-ttu-id="b5f3d-114">**Disponibilidade do calendário com as horas, o assunto e a localização**</span><span class="sxs-lookup"><span data-stu-id="b5f3d-114">**Calendar free/busy with time, subject, and location**</span></span>  

 <span data-ttu-id="b5f3d-115">Para definir os utilizadores que irão partilhar informações de disponibilidade do calendário, selecione uma das seguintes opções:</span><span class="sxs-lookup"><span data-stu-id="b5f3d-115">To set which users will share calendar free/busy information, select one of the following:</span></span>

- <span data-ttu-id="b5f3d-116">**Todas as pessoas na sua organização**</span><span class="sxs-lookup"><span data-stu-id="b5f3d-116">**Everyone in your organization**</span></span>
- <span data-ttu-id="b5f3d-117">**Um grupo de segurança específico**</span><span class="sxs-lookup"><span data-stu-id="b5f3d-117">**A specified security group**</span></span>  

<span data-ttu-id="b5f3d-118">Clique **procurar** para escolher o grupo de segurança a partir de uma lista e, em seguida, clique em **ok**.</span><span class="sxs-lookup"><span data-stu-id="b5f3d-118">Click **browse** to pick the security group from a list, then click **ok**.</span></span>

<span data-ttu-id="b5f3d-119">Clique em **guardar** para criar a relação da organização.</span><span class="sxs-lookup"><span data-stu-id="b5f3d-119">Click **save** to create the organization relationship.</span></span>  

<span data-ttu-id="b5f3d-120">**Nota:** Configurações entre inquilinos não suportam contactos pessoais para pesquisa de disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="b5f3d-120">**Note:** Cross-tenant configurations do not support personal contacts for free/busy lookup.</span></span> <span data-ttu-id="b5f3d-121">Os contactos têm de ser incluídos na lista de endereços global para que a pesquisa de disponibilidade funcione.</span><span class="sxs-lookup"><span data-stu-id="b5f3d-121">Contacts must be included in the global address list for free/busy lookup to work.</span></span>

<span data-ttu-id="b5f3d-122">**Para compreender este tópico de forma aprofundada, consulte:**</span><span class="sxs-lookup"><span data-stu-id="b5f3d-122">**For full understanding of this topic please read:**</span></span>

- [<span data-ttu-id="b5f3d-123">Criar uma relação da organização no Exchange Online</span><span class="sxs-lookup"><span data-stu-id="b5f3d-123">Create an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/create-an-organization-relationship)
- [<span data-ttu-id="b5f3d-124">Modificar uma relação da organização no Exchange Online</span><span class="sxs-lookup"><span data-stu-id="b5f3d-124">Modify an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/modify-an-organization-relationship)
- [<span data-ttu-id="b5f3d-125">Remover uma relação da organização no Exchange Online</span><span class="sxs-lookup"><span data-stu-id="b5f3d-125">Remove an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/remove-an-organization-relationship)
