---
title: Encontrar eventos realizados nas regras da caixa de entrada
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: deb83d278a2b398b4ea6fc31b043c33309b736e3
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430013"
---
# <a name="find-events-performed-on-inbox-rules"></a><span data-ttu-id="6f1b0-102">Encontrar eventos realizados nas regras da caixa de entrada</span><span class="sxs-lookup"><span data-stu-id="6f1b0-102">Find events performed on inbox rules</span></span>

<span data-ttu-id="6f1b0-103">Quando as regras da caixa de entrada são criadas, alteradas ou eliminadas, os eventos são registados no registo de auditoria.</span><span class="sxs-lookup"><span data-stu-id="6f1b0-103">When inbox rules are created, changed, or deleted, the events are recorded in the audit log.</span></span> <span data-ttu-id="6f1b0-104">Eis como revê-los:</span><span class="sxs-lookup"><span data-stu-id="6f1b0-104">Here's how to review them:</span></span>

1. <span data-ttu-id="6f1b0-105">Vá ao [Centro de Segurança & Compliance do Office 365.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="6f1b0-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="6f1b0-106">Selecione Pesquisar > Audit pesquisa de registo.</span><span class="sxs-lookup"><span data-stu-id="6f1b0-106">Select Search > Audit log search.</span></span>

    > [!NOTE]
    > <span data-ttu-id="6f1b0-107">Se vir um aviso de que precisa de ligar a auditoria, vá em frente e ligue-o agora.</span><span class="sxs-lookup"><span data-stu-id="6f1b0-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="6f1b0-108">Se esta funcionalidade não estiver ligada, os resultados da pesquisa não serão capazes de extrair dados de datas anteriores.</span><span class="sxs-lookup"><span data-stu-id="6f1b0-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="6f1b0-109">Selecione o campo Atividades e encontre as atividades da caixa de correio de Troca e, em seguida, selecione New-InboxRule Criar regra de caixa de entrada a partir da App Web do Outlook.</span><span class="sxs-lookup"><span data-stu-id="6f1b0-109">Select the Activities field and find Exchange mailbox activities, and then select New-InboxRule Create inbox rule from Outlook Web App.</span></span> <span data-ttu-id="6f1b0-110">Quando terminar, clique fora do painel para minimizar o painel de Atividades.</span><span class="sxs-lookup"><span data-stu-id="6f1b0-110">When you're done, click outside of the pane to minimize the Activities pane.</span></span>
1. <span data-ttu-id="6f1b0-111">Especifique o intervalo de datas e, em seguida, no campo Utilizadores, selecione o nome de utilizador para o utilizador que pretende investigar.</span><span class="sxs-lookup"><span data-stu-id="6f1b0-111">Specify the date range, and then in the Users field, select the username for the user you want to investigate.</span></span> <span data-ttu-id="6f1b0-112">Pode selecionar mais do que um utilizador de cada vez.</span><span class="sxs-lookup"><span data-stu-id="6f1b0-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="6f1b0-113">Selecione Pesquisar.</span><span class="sxs-lookup"><span data-stu-id="6f1b0-113">Select Search.</span></span> <span data-ttu-id="6f1b0-114">As atividades aparecem nos Resultados.</span><span class="sxs-lookup"><span data-stu-id="6f1b0-114">The activities appear under Results.</span></span>
1. <span data-ttu-id="6f1b0-115">Para ver detalhes, selecione uma atividade e, em seguida, selecione Mais Informações.</span><span class="sxs-lookup"><span data-stu-id="6f1b0-115">To view details, select an activity, and then select More Information.</span></span> <span data-ttu-id="6f1b0-116">Na secção Parâmetros pode ver o nome da regra, as condições definidas e as ações que a regra irá tomar.</span><span class="sxs-lookup"><span data-stu-id="6f1b0-116">Under the Parameters section you can see the name of the rule, conditions set, and the actions that the rule will take.</span></span>

<span data-ttu-id="6f1b0-117">Para saber mais, consulte o registo de auditoria do Office 365 para resolver cenários comuns.</span><span class="sxs-lookup"><span data-stu-id="6f1b0-117">To learn more, see Search the Office 365 audit log to troubleshoot common scenarios.</span></span>