---
title: Problema com um único utilizador
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8469"
ms.openlocfilehash: f3564063a3adf291ec4909ffeb2f6de0e478da96
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430203"
---
# <a name="problem-with-single-user"></a><span data-ttu-id="a803b-102">Problema com um único utilizador</span><span class="sxs-lookup"><span data-stu-id="a803b-102">Problem with single user</span></span>

- <span data-ttu-id="a803b-103">O utilizador pode não ter sido prestado porque o serviço ainda não teve oportunidade de avaliar o utilizador.</span><span class="sxs-lookup"><span data-stu-id="a803b-103">The user may not have been provisioned because the service hasn't had a chance to evaluate the user yet.</span></span> <span data-ttu-id="a803b-104">Reveja as orientações para o tempo de provisão, bem como a barra de progresso na página de configuração de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="a803b-104">Review the guidance for how long provisioning takes as well as the progress bar on the provisioning configuration page.</span></span> <span data-ttu-id="a803b-105">Se o estado estacionário especificado na secção de detalhes adicionais for antes da data em que o utilizador foi criado/atualizado/eliminado, significa que ainda não avaliámos o utilizador.</span><span class="sxs-lookup"><span data-stu-id="a803b-105">If the steady state specified in the additional details section is before the date the user was created/updated/deleted, it means we have not evaluated the user yet.</span></span> <span data-ttu-id="a803b-106">Neste cenário, a melhor coisa a fazer é esperar que o serviço de prestação termine.</span><span class="sxs-lookup"><span data-stu-id="a803b-106">In this scenario, the best thing to do is wait for the provisioning service to finish.</span></span>

  - <span data-ttu-id="a803b-107">Note que o nosso serviço só tem conhecimento de alterações a um utilizador no sistema de origem (Cloud HR).</span><span class="sxs-lookup"><span data-stu-id="a803b-107">Note that our service is only aware of changes to a user in the source system (Cloud HR).</span></span> <span data-ttu-id="a803b-108">Tem de haver uma alteração válida no sistema de origem para a Azure AD detetar a mudança e fluí-la para o Ative Directory.</span><span class="sxs-lookup"><span data-stu-id="a803b-108">There has to be a valid change in the source system for Azure AD to detect the change and flow it into Active Directory.</span></span>
- <span data-ttu-id="a803b-109">O serviço de prestação avaliou o utilizador e determinou que não deveria ser a provisionado:</span><span class="sxs-lookup"><span data-stu-id="a803b-109">Provisioning service evaluated the user and determined it should not be provisioned:</span></span>
  - <span data-ttu-id="a803b-110">Se tiver definido um filtro de deteção baseado em atributos, certifique-se de que o utilizador satisfaz os critérios especificados.</span><span class="sxs-lookup"><span data-stu-id="a803b-110">If you have set an attribute based scoping filter, ensure that the user meets the criteria that you have specified.</span></span>
  - <span data-ttu-id="a803b-111">Se os utilizadores já existirem no sistema-alvo e no estado do utilizador na origem e no target match, não tomaremos mais nenhuma ação.</span><span class="sxs-lookup"><span data-stu-id="a803b-111">If users already exist in the target system and the state of the user in the source and target match, we won't take any further action.</span></span>
- <span data-ttu-id="a803b-112">O serviço de fornecimento tentou forrar o utilizador e falhou.</span><span class="sxs-lookup"><span data-stu-id="a803b-112">Provisioning service attempted to provision the user and it failed.</span></span> <span data-ttu-id="a803b-113">Para estes cenários, reveja o separador de resolução de problemas e recomendações dos registos de provisionamento:</span><span class="sxs-lookup"><span data-stu-id="a803b-113">For these scenarios, review the troubleshooting and recommendations tab of the provisioning logs:</span></span>
  - <span data-ttu-id="a803b-114">Um atributo necessário para o utilizador pode estar em falta no Ative Directory ou Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a803b-114">A required attribute on the user might be missing in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="a803b-115">Por exemplo, as regras de geração do userPrincipalName ou sAMAccountName não estão a gerar o valor certo.</span><span class="sxs-lookup"><span data-stu-id="a803b-115">For example, the userPrincipalName or sAMAccountName generation rules are not generating the right value.</span></span>
  - <span data-ttu-id="a803b-116">O atributo correspondente (geralmente employeeId) não está a ser resolvida para um utilizador único no Ative Directory ou AZure AD.</span><span class="sxs-lookup"><span data-stu-id="a803b-116">The matching attribute (usually employeeId) is not resolving to a unique user in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="a803b-117">Por exemplo, existem dois utilizadores com o mesmo colaboradorId em AD e o serviço devolve um código de erro indica entradas-alvo duplicadas para a mesma entrada de origem.</span><span class="sxs-lookup"><span data-stu-id="a803b-117">For example, there are two users with the same employeeId in AD and the service returns an error code indicate duplicate target entries for the same source entry.</span></span>

<span data-ttu-id="a803b-118">Para rever os registos de um único utilizador e grupos, consulte [rever os registos de provisionamento para um problema com um utilizador específico](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).</span><span class="sxs-lookup"><span data-stu-id="a803b-118">To review logs for single user and groups, see [Review the provisioning logs for an issue with a specific user](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).</span></span>
