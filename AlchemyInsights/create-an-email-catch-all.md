---
title: Criar um e-mail catch all
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 262d2c6a7181d94094f3d840c4ba3ebd07000cf4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712997"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="1aea9-102">Criar um e-mail catch all</span><span class="sxs-lookup"><span data-stu-id="1aea9-102">Create an email catch all</span></span>

<span data-ttu-id="1aea9-103">A utilização de uma captura é fortemente desencorajada.</span><span class="sxs-lookup"><span data-stu-id="1aea9-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="1aea9-104">É melhor dar um salto de volta ao remetente, informando os remetentes que a sua mensagem não possa ser entregue como endereçado, para que possam tomar medidas.</span><span class="sxs-lookup"><span data-stu-id="1aea9-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="1aea9-105">Também pode limitar a caixa de correio monitorizada apenas para capturar endereços de e-mail anteriormente válidos.</span><span class="sxs-lookup"><span data-stu-id="1aea9-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="1aea9-106">Qualquer captura de toda a caixa de correio receberá uma boa dose de spam e poderá eventualmente preencher se não for monitorizada de perto.</span><span class="sxs-lookup"><span data-stu-id="1aea9-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="1aea9-107">(Existem limites de receção.)</span><span class="sxs-lookup"><span data-stu-id="1aea9-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="1aea9-108">Se decidir prosseguir, siga estes passos:</span><span class="sxs-lookup"><span data-stu-id="1aea9-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="1aea9-109">Criar um grupo de distribuição dinâmica & inclua "Todos os tipos de destinatários".</span><span class="sxs-lookup"><span data-stu-id="1aea9-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="1aea9-110">Crie uma caixa de correio dedicada para apanhar e-mails, por exemplo, catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="1aea9-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="1aea9-111">Para o domínio específico, desaprote o 'DomainType' para "InternalRelay".</span><span class="sxs-lookup"><span data-stu-id="1aea9-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="1aea9-112">Se mais tarde retirar todas as capturas, certifique-se de que devolve o domínio ao Autoritário.</span><span class="sxs-lookup"><span data-stu-id="1aea9-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="1aea9-113">Criar uma Regra de Transporte de Fluxo de Correio da seguinte forma:</span><span class="sxs-lookup"><span data-stu-id="1aea9-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="1aea9-114">Se o Remetente estiver "Fora da Organização"</span><span class="sxs-lookup"><span data-stu-id="1aea9-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="1aea9-115">Redirecione a mensagem para Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="1aea9-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="1aea9-116">Exceto se o destinatário for membro da allusers@domain.com (o Grupo de Distribuição contém todos os membros)</span><span class="sxs-lookup"><span data-stu-id="1aea9-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="1aea9-117">Certifique-se de validar que novas caixas de correio são adicionadas ao Grupo de Distribuição Dinâmica</span><span class="sxs-lookup"><span data-stu-id="1aea9-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
