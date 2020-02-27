---
title: Criar um e-mail catch all
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 35f31c1662547d57c2fc9978ffb495ac29abcc01
ms.sourcegitcommit: 67015549afcbe05f3b77ea314e2ef7e0e439f9f2
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/26/2020
ms.locfileid: "42286203"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="25b84-102">Criar um e-mail catch all</span><span class="sxs-lookup"><span data-stu-id="25b84-102">Create an email catch all</span></span>

<span data-ttu-id="25b84-103">A utilização de uma captura é fortemente desencorajada.</span><span class="sxs-lookup"><span data-stu-id="25b84-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="25b84-104">É melhor dar um salto de volta ao remetente, deixando os remetentes saberem que a sua mensagem não poderia ser entregue como endereçada para que possam tomar medidas.</span><span class="sxs-lookup"><span data-stu-id="25b84-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="25b84-105">Também pode limitar a caixa de correio monitorizada apenas para capturar endereços de e-mail anteriormente válidos.</span><span class="sxs-lookup"><span data-stu-id="25b84-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="25b84-106">Qualquer captura, todas as caixas de correio receberão uma boa dose de spam e poderão eventualmente preencher se não forem monitorizadas de perto.</span><span class="sxs-lookup"><span data-stu-id="25b84-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="25b84-107">(Há limites de receção.)</span><span class="sxs-lookup"><span data-stu-id="25b84-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="25b84-108">Se decidir prosseguir, siga estes passos:</span><span class="sxs-lookup"><span data-stu-id="25b84-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="25b84-109">Criar um Grupo de Distribuição Dinâmica & incluir "Todos os tipos de destinatários".</span><span class="sxs-lookup"><span data-stu-id="25b84-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="25b84-110">Crie uma Caixa de Correio dedicada para apanhar e-mails, por exemplo, catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="25b84-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="25b84-111">Para o domínio específico, desloque o DomainType para "InternalRelay".</span><span class="sxs-lookup"><span data-stu-id="25b84-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="25b84-112">Se remover mais tarde a captura, certifique-se de que o domínio volta a ser Autorizado.</span><span class="sxs-lookup"><span data-stu-id="25b84-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="25b84-113">Crie uma Regra de Transporte de Fluxos de Correio da seguinte forma:</span><span class="sxs-lookup"><span data-stu-id="25b84-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="25b84-114">Se o Remetente estiver "Fora da Organização"</span><span class="sxs-lookup"><span data-stu-id="25b84-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="25b84-115">Redirecione a mensagem para Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="25b84-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="25b84-116">Exceto se o destinatário for membro da allusers@domain.com (Grupo de Distribuição contém todos os membros)</span><span class="sxs-lookup"><span data-stu-id="25b84-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="25b84-117">Certifique-se de validar que novas caixas de correio são adicionadas ao Grupo de Distribuição Dinâmica</span><span class="sxs-lookup"><span data-stu-id="25b84-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
