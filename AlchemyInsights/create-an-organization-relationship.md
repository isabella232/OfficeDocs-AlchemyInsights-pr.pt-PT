---
title: Crie uma Relação de Organização para permitir que os seus utilizadores colaborem com outra organização
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 2c6cd6a178c6e012bfe1c8d769b037168ffa3254
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862197"
---
# <a name="create-an-organization-relationship-to-allow-your-users-to-collaborate-with-another-organization"></a><span data-ttu-id="7dc78-102">Crie uma Relação de Organização para permitir que os seus utilizadores colaborem com outra organização</span><span class="sxs-lookup"><span data-stu-id="7dc78-102">Create an Organization Relationship to allow your users to collaborate with another organization</span></span>

1. <span data-ttu-id="7dc78-103">A partir do painel central de administração microsoft 365, vá ao **Admin**  >  **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="7dc78-103">From the Microsoft 365 admin center dashboard, go to **Admin** > **Exchange**.</span></span>
2. <span data-ttu-id="7dc78-104">Vá à **partilha de organizações.**  >  **sharing**</span><span class="sxs-lookup"><span data-stu-id="7dc78-104">Go to **organization** > **sharing**.</span></span>
3. <span data-ttu-id="7dc78-105">Em **Partilha de Organização,** clique em **New** .</span><span class="sxs-lookup"><span data-stu-id="7dc78-105">Under **Organization Sharing**, click **New** .</span></span>
4. <span data-ttu-id="7dc78-106">Na **nova relação de organização,** na caixa de **nomes relacionamento,** escreva um nome amigável para a relação de organização.</span><span class="sxs-lookup"><span data-stu-id="7dc78-106">In **new organization relationship**, in the **Relationship name** box, type a friendly name for the organization relationship.</span></span>
5. <span data-ttu-id="7dc78-107">Nos **Domínios para partilhar com** a caixa, digite o domínio para a organização externa do Office 365 ou Exchange on-ins que pretende deixar ver os seus calendários.</span><span class="sxs-lookup"><span data-stu-id="7dc78-107">In the **Domains to share with** box, type the domain for the external Office 365 or Exchange on-premises organization you want to let see your calendars.</span></span> <span data-ttu-id="7dc78-108">Se precisar de introduzir mais de um domínio, separe os nomes de domínio com uma vírgula.</span><span class="sxs-lookup"><span data-stu-id="7dc78-108">If you need to enter more than one domain, separate the domain names with a comma.</span></span> <span data-ttu-id="7dc78-109">Por exemplo, contoso.com, service.contoso.com.</span><span class="sxs-lookup"><span data-stu-id="7dc78-109">For example, contoso.com, service.contoso.com.</span></span>
6. <span data-ttu-id="7dc78-110">Selecione a caixa **de verificação de partilha de informações free/busy do calendário** para ligar a partilha do calendário com os domínios listados.</span><span class="sxs-lookup"><span data-stu-id="7dc78-110">Select the **Enable calendar free/busy information sharing** check box to turn on calendar sharing with the domains you listed.</span></span> <span data-ttu-id="7dc78-111">Desafete o nível de partilha para informações gratuitas/ocupadas do calendário e definir quais os utilizadores que possam partilhar informações gratuitas/ocupadas do calendário.</span><span class="sxs-lookup"><span data-stu-id="7dc78-111">Set the sharing level for calendar free/busy information and set which users can share calendar free/busy information.</span></span>  

<span data-ttu-id="7dc78-112">Para definir o nível de acesso livre/ocupado, selecione um dos seguintes:</span><span class="sxs-lookup"><span data-stu-id="7dc78-112">To set the free/busy access level, select one of the following:</span></span>

- <span data-ttu-id="7dc78-113">**Informações de disponibilidade do calendário apenas com as horas**</span><span class="sxs-lookup"><span data-stu-id="7dc78-113">**Calendar free/busy information with time only**</span></span>
- <span data-ttu-id="7dc78-114">**Calendário livre/ocupado com tempo, assunto e localização**</span><span class="sxs-lookup"><span data-stu-id="7dc78-114">**Calendar free/busy with time, subject, and location**</span></span>  

 <span data-ttu-id="7dc78-115">Para definir quais os utilizadores que partilharão informações gratuitas/ocupadas do calendário, selecione uma das seguintes:</span><span class="sxs-lookup"><span data-stu-id="7dc78-115">To set which users will share calendar free/busy information, select one of the following:</span></span>

- <span data-ttu-id="7dc78-116">**Todos na sua organização**</span><span class="sxs-lookup"><span data-stu-id="7dc78-116">**Everyone in your organization**</span></span>
- <span data-ttu-id="7dc78-117">**Um grupo de segurança especificado**</span><span class="sxs-lookup"><span data-stu-id="7dc78-117">**A specified security group**</span></span>  

<span data-ttu-id="7dc78-118">Clique **em procurar** para escolher o grupo de segurança de uma lista e, em seguida, clique em **ok**.</span><span class="sxs-lookup"><span data-stu-id="7dc78-118">Click **browse** to pick the security group from a list, then click **ok**.</span></span>

<span data-ttu-id="7dc78-119">Clique **em guardar** para criar a relação de organização.</span><span class="sxs-lookup"><span data-stu-id="7dc78-119">Click **save** to create the organization relationship.</span></span>  

<span data-ttu-id="7dc78-120">**Nota:** As configurações de inquilinos cruzados não suportam contactos pessoais para uma procura gratuita/ocupada.</span><span class="sxs-lookup"><span data-stu-id="7dc78-120">**Note:** Cross-tenant configurations do not support personal contacts for free/busy lookup.</span></span> <span data-ttu-id="7dc78-121">Os contactos devem ser incluídos na lista de endereços globais para uma procura gratuita/ocupada para trabalhar.</span><span class="sxs-lookup"><span data-stu-id="7dc78-121">Contacts must be included in the global address list for free/busy lookup to work.</span></span>

<span data-ttu-id="7dc78-122">**Para uma compreensão completa deste tópico, leia:**</span><span class="sxs-lookup"><span data-stu-id="7dc78-122">**For full understanding of this topic please read:**</span></span>

- [<span data-ttu-id="7dc78-123">Criar uma relação de organização em Exchange Online</span><span class="sxs-lookup"><span data-stu-id="7dc78-123">Create an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/create-an-organization-relationship)
- [<span data-ttu-id="7dc78-124">Modifique uma relação de organização em Exchange Online</span><span class="sxs-lookup"><span data-stu-id="7dc78-124">Modify an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/modify-an-organization-relationship)
- [<span data-ttu-id="7dc78-125">Remover uma relação de organização em Exchange Online</span><span class="sxs-lookup"><span data-stu-id="7dc78-125">Remove an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/remove-an-organization-relationship)
