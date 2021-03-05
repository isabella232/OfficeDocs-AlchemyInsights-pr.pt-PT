---
title: Problema com atributo e filtro de scoping
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8470"
- "9004687"
ms.openlocfilehash: 78df24c0d8a670d678e26879cf81476f1ae9b92d
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481898"
---
# <a name="problem-with-attribute-and-scoping-filter"></a><span data-ttu-id="e4b34-102">Problema com atributo e filtro de scoping</span><span class="sxs-lookup"><span data-stu-id="e4b34-102">Problem with attribute and scoping filter</span></span>

<span data-ttu-id="e4b34-103">**Problema com valores de UPN em conflito**</span><span class="sxs-lookup"><span data-stu-id="e4b34-103">**Issue with conflicting UPN values**</span></span>

<span data-ttu-id="e4b34-104">O Workday to AD User Provisioning Workday to AD User Provisioning mostra mensagem de erro **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**.</span><span class="sxs-lookup"><span data-stu-id="e4b34-104">The Workday to AD User Provisioning Workday to AD User Provisioning shows error message **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**.</span></span> <span data-ttu-id="e4b34-105">A operação falhou porque o valor UPN previsto para a adição/modificação não é único em toda a floresta.</span><span class="sxs-lookup"><span data-stu-id="e4b34-105">The operation failed because UPN value provided for addition/modification is not unique forest-wide.</span></span> <span data-ttu-id="e4b34-106">Detalhes de erro: **CONSTRAINT_ATT_TYPE - userPrincipalName**.</span><span class="sxs-lookup"><span data-stu-id="e4b34-106">Error Details: **CONSTRAINT_ATT_TYPE - userPrincipalName**.</span></span>

<span data-ttu-id="e4b34-107">O **valor do nome Do utilizadorPrincipal Que** o conector Workday está a tentar definir ao criar a conta de utilizador AD já existe no domínio de AD alvo.</span><span class="sxs-lookup"><span data-stu-id="e4b34-107">The **userPrincipalName** value that Workday connector is trying to set when creating the AD user account already exists in the target AD domain.</span></span> <span data-ttu-id="e4b34-108">Isto implica que ou (1) o utilizador já existe e a verificação de identificação correspondente falhou para o utilizador ou (2) a regra de geração UPN gerou um valor conflituoso.</span><span class="sxs-lookup"><span data-stu-id="e4b34-108">This implies that either (1) the user already exists and the matching ID check failed for the user or (2) the UPN generation rule generated a conflicting value.</span></span>

<span data-ttu-id="e4b34-109">Aqui estão as etapas de resolução sugeridas:</span><span class="sxs-lookup"><span data-stu-id="e4b34-109">Here are the suggested resolution steps:</span></span>

<span data-ttu-id="e4b34-110">Se o utilizador já existe e o controlo de identificação correspondente não conseguiu ligar a conta Workday à conta Ative Directory, verifique se o atributo ID correspondente (normalmente **funcionárioID)** em ambos os dias de trabalho e AD tem uma correspondência exata.</span><span class="sxs-lookup"><span data-stu-id="e4b34-110">If the user already exists and the matching ID check failed to link the Workday account to Active Directory account, then check if the matching ID attribute (typically **employeeID**) in both Workday and AD have an exact match.</span></span> <span data-ttu-id="e4b34-111">Se não tiverem correspondência, é uma questão de dados que tem de ser corrigida.</span><span class="sxs-lookup"><span data-stu-id="e4b34-111">If they don't have a match, it is a data issue that needs to be fixed.</span></span> <span data-ttu-id="e4b34-112">Por exemplo, se o EmployeeID no Workday for 001052 e em AD é 1052, então o motor de provisionamento não ligará as duas contas e tentará criar um utilizador que já exista.</span><span class="sxs-lookup"><span data-stu-id="e4b34-112">For example, if the EmployeeID in Workday is 001052 and in AD it is 1052, then the provisioning engine will fail to link the two accounts and will try to create a user that already exists.</span></span> <span data-ttu-id="e4b34-113">A solução neste caso é alterar o valor **do EmployeeID** em AD para incluir os principais zeros para torná-lo 001052.</span><span class="sxs-lookup"><span data-stu-id="e4b34-113">The solution in this case is to change the **EmployeeID** value in AD to include the leading zeros to make it 001052.</span></span>
<span data-ttu-id="e4b34-114">Se a expressão geradora da UPN não estiver a gerar um valor único, considere usar a função de des **duplicação SelectUniqueValue** para gerar um valor único cada vez.</span><span class="sxs-lookup"><span data-stu-id="e4b34-114">If the UPN-generating expression is not generating a unique value, consider using the de-duplication function **SelectUniqueValue** to generate a unique value each time.</span></span>

<span data-ttu-id="e4b34-115">**O dia de trabalho para o Fornecimento de Utilizadores AD não define o valor do atributo do gestor para a conta de utilizador de AD**</span><span class="sxs-lookup"><span data-stu-id="e4b34-115">**Workday to AD User Provisioning does not set manager attribute value for AD user account**</span></span>

<span data-ttu-id="e4b34-116">O trabalho de Provisão de utilizadores de trabalho para AD não está a definir o valor do atributo **do gestor** para contas de utilizador de AD.</span><span class="sxs-lookup"><span data-stu-id="e4b34-116">The Workday to AD User Provisioning job is not setting the **manager** attribute value for AD user accounts.</span></span> <span data-ttu-id="e4b34-117">Há dois cenários possíveis quando este comportamento é visto:</span><span class="sxs-lookup"><span data-stu-id="e4b34-117">There are two possible scenarios when this behavior is seen:</span></span>

1. <span data-ttu-id="e4b34-118">O gestor em Workday não pode ser resolvido para uma conta de Utilizador AD correspondente porque o gestor não está no âmbito.</span><span class="sxs-lookup"><span data-stu-id="e4b34-118">The manager in Workday cannot be resolved to a corresponding AD User account because the manager is not in scope.</span></span>
2. <span data-ttu-id="e4b34-119">Num cenário **de vários domínios de AD,** o gestor em Workday não está presente no mesmo domínio que o utilizador.</span><span class="sxs-lookup"><span data-stu-id="e4b34-119">In a **multiple AD domains** scenario, the manager in Workday is not present in the same domain as the user.</span></span>

<span data-ttu-id="e4b34-120">Experimente estes passos para resolver a questão:</span><span class="sxs-lookup"><span data-stu-id="e4b34-120">Try these steps to resolve the issue:</span></span>

1. <span data-ttu-id="e4b34-121">Se tiver definido filtros de deteção, verifique primeiro se o gestor está no âmbito e se satisfaz a cláusula de deteção.</span><span class="sxs-lookup"><span data-stu-id="e4b34-121">If you have defined scoping filters, first check if the manager is in scope and that it satisfies the scoping clause.</span></span> <span data-ttu-id="e4b34-122">Se o gestor não satisfizer o filtro de escoamento, mude o filtro de modo a que o gestor também esteja no âmbito da operação de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="e4b34-122">If the manager does not satisfy the scoping filter, change the filter so that the manager is also in scope of the provisioning operation.</span></span>
2. <span data-ttu-id="e4b34-123">Se tiver vários domínios de AD, então o conector tem uma limitação conhecida da incapacidade de resolver referências de gestor de domínio transversal.</span><span class="sxs-lookup"><span data-stu-id="e4b34-123">If you have multiple AD domains, then the connector has a known limitation of inability to resolve cross-domain manager references.</span></span>

<span data-ttu-id="e4b34-124">Para obter mais informações sobre a configuração do dia de trabalho para o provisionamento automatizado, consulte [Tutorial: Configure Workday para o provisionamento automático do utilizador](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="e4b34-124">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>













