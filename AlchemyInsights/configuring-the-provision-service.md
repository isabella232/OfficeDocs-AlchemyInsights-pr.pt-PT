---
title: Configuração do serviço de Provisão
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
- "8468"
ms.openlocfilehash: fd272f8d554d73c87b832443815c25ebb2acc3eb
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/05/2021
ms.locfileid: "50484050"
---
# <a name="configuring-the-provision-service"></a><span data-ttu-id="e3e2a-102">Configuração do serviço de Provisão</span><span class="sxs-lookup"><span data-stu-id="e3e2a-102">Configuring the Provision service</span></span>

<span data-ttu-id="e3e2a-103">Para o fornecimento automatizado de utilizadores para funcionar, o Azure AD requer credenciais válidas que lhe permitem ligar-se à API dos Serviços Web workday.</span><span class="sxs-lookup"><span data-stu-id="e3e2a-103">For automated user provisioning to work, Azure AD requires valid credentials that allow it to connect to Workday Web Services API.</span></span> <span data-ttu-id="e3e2a-104">Além disso, o botão de Ligação de Teste no Dia de Trabalho para a aplicação de provisionamento do utilizador AD também valida se for capaz de se ligar ao Agente de Provisionamento AD AD Ad associado ao Domínio AD.</span><span class="sxs-lookup"><span data-stu-id="e3e2a-104">Further, the Test Connection button on the Workday to AD User Provisioning app also validates if it is able to connect to the Azure AD Connect Provisioning Agent associated with the AD Domain.</span></span>

<span data-ttu-id="e3e2a-105">Se o portal Azure estiver a devolver um erro ao guardar as credenciais, siga os passos recomendados abaixo:</span><span class="sxs-lookup"><span data-stu-id="e3e2a-105">If the Azure portal is returning an error upon saving the credentials, follow the recommended steps below:</span></span>

1. <span data-ttu-id="e3e2a-106">Confirme que configura a conta do Utilizador do Sistema de Integração workday, conforme indicado na secção tutorial [Configure o utilizador do sistema de integração no Workday](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="e3e2a-106">Confirm that you have configured Workday Integration System User account as stated in the tutorial section [Configure integration system user in Workday](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
2. <span data-ttu-id="e3e2a-107">Confirme que o Serviço de Agente de Provisionamento AD AD AZure está a funcionar no seu servidor Windows no local utilizando a Consola de Gestão de Serviços.</span><span class="sxs-lookup"><span data-stu-id="e3e2a-107">Confirm that the Azure AD Connect Provisioning Agent Service is up and running on your on-premises Windows server using the Services Management Console.</span></span> <span data-ttu-id="e3e2a-108">Também pode verificar o estado do agente no portal Azure clicando no botão Ver agentes no local.</span><span class="sxs-lookup"><span data-stu-id="e3e2a-108">You can also check the status of the agent in the Azure portal by clicking the View on-premises agents button.</span></span>
3. <span data-ttu-id="e3e2a-109">Certifique-se de que está a introduzir o valor para o campo "Nome de Utilizador workday" utilizando o formato username@workday-nome de inquilino.</span><span class="sxs-lookup"><span data-stu-id="e3e2a-109">Ensure that you are entering the value for "Workday Username" field using the format username@workday-tenant-name.</span></span> <span data-ttu-id="e3e2a-110">Se faltar o nome do inquilino do dia de trabalho, a autenticação do workday falha.</span><span class="sxs-lookup"><span data-stu-id="e3e2a-110">If the workday-tenant-name is missing, Workday authentication fails.</span></span>
4. <span data-ttu-id="e3e2a-111">Se estiver a configurar a integração com o inquilino de implementação workday, observe as horas de inatividade programadas do seu inquilino workday.</span><span class="sxs-lookup"><span data-stu-id="e3e2a-111">If you are configuring the integration with Workday implementation tenant, note the scheduled downtime hours of your Workday tenant.</span></span> <span data-ttu-id="e3e2a-112">O workday tem programado tempo de inatividade para os seus inquilinos de implementação durante os fins de semana (geralmente de sexta-feira à noite para sábado de manhã) e falhas de conectividade durante esta janela de tempo de inatividade é uma questão conhecida que resolve automaticamente assim que os inquilinos de implementação estão novamente on-line.</span><span class="sxs-lookup"><span data-stu-id="e3e2a-112">Workday has scheduled down time for its implementation tenants over weekends (usually from Friday evening to Saturday morning) and connectivity failures during this downtime window is a known issue that auto-resolves as soon as the implementation tenants are back online.</span></span>
5. <span data-ttu-id="e3e2a-113">Em casos raros, poderá também ver este erro se a palavra-passe do Utilizador do Sistema de Integração for alterada devido à atualização do arrendatário ou se a conta estiver em estado fechado ou caducado.</span><span class="sxs-lookup"><span data-stu-id="e3e2a-113">In rare cases, you may also see this error if the password of the Integration System User changed due to tenant refresh or if the account is in locked or expired state.</span></span> <span data-ttu-id="e3e2a-114">Verifique o estado do utilizador do Sistema de Integração com o seu administrador workday.</span><span class="sxs-lookup"><span data-stu-id="e3e2a-114">Please check the status of the Integration System user with your Workday administrator.</span></span>

<span data-ttu-id="e3e2a-115">Para obter mais informações sobre a configuração do dia de trabalho para o provisionamento automatizado, consulte [Tutorial: Configure Workday para o provisionamento automático do utilizador](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="e3e2a-115">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
