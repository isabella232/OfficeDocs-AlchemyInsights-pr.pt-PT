---
title: Identificar excluir eventos de mensagens em registos de auditoria
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: bc78076706aee15a3133c4b1a89064591f790b58
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696524"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="b937e-102">Registos de auditoria para mensagens de correio de correio de correio apagados</span><span class="sxs-lookup"><span data-stu-id="b937e-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="b937e-103">A partir de janeiro de 2019, a Microsoft está a ligar a auditoria da caixa de correio por padrão.</span><span class="sxs-lookup"><span data-stu-id="b937e-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="b937e-104">Caso contrário, para rever os eventos de mensagens para um utilizador específico, é necessário ativar manualmente as ações de eliminação para auditoria.</span><span class="sxs-lookup"><span data-stu-id="b937e-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="b937e-105">Se o registo de auditoria da caixa de correio já estiver ativado para a sua organização ou para o utilizador específico, siga os passos abaixo.</span><span class="sxs-lookup"><span data-stu-id="b937e-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="b937e-106">Faça login no [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="b937e-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="b937e-107">Clique em **Pesquisar e Investigar** e selecione Audit Log **Search**.</span><span class="sxs-lookup"><span data-stu-id="b937e-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="b937e-108">Selecione o intervalo de datas nos campos **data de início** e **fim.**</span><span class="sxs-lookup"><span data-stu-id="b937e-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="b937e-109">Especifique o nome de utilizador para o utilizador que pretende investigar (o utilizador que eliminou os itens).</span><span class="sxs-lookup"><span data-stu-id="b937e-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="b937e-110">No campo **Atividades,** **selecione mensagens eliminadas da pasta de itens eliminados** e **mensagens movidas para pasta de Itens Eliminados**.</span><span class="sxs-lookup"><span data-stu-id="b937e-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="b937e-111">Clique **em Pesquisar**.</span><span class="sxs-lookup"><span data-stu-id="b937e-111">Click **Search**.</span></span>

<span data-ttu-id="b937e-112">Nos resultados, selecione um registo de auditoria.</span><span class="sxs-lookup"><span data-stu-id="b937e-112">In the results, select an audit record.</span></span> <span data-ttu-id="b937e-113">No voo de informação, clique em **Mais Informações.**</span><span class="sxs-lookup"><span data-stu-id="b937e-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="b937e-114">Informações adicionais sobre o item eliminado (por exemplo, a linha de assunto e a localização do item quando foi eliminado) são apresentadas no campo **AffectedItems.**</span><span class="sxs-lookup"><span data-stu-id="b937e-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="b937e-115">A propriedade **ClientInfoString** mostrará se a eliminação ocorreu no Outlook, Outlook na web (anteriormente conhecida como Outlook Web App), ou qualquer outro dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b937e-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="b937e-116">Para obter mais informações, consulte [Determineing quem criou o reencaminhamento de e-mail para uma caixa de correio](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="b937e-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="b937e-117">**Nota:** Não é possível recuperar itens eliminados utilizando a função de registo de auditoria.</span><span class="sxs-lookup"><span data-stu-id="b937e-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="b937e-118">Para obter mensagens eliminadas no Outlook na web, consulte [Recuperar itens eliminados na App Web do Outlook](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="b937e-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
