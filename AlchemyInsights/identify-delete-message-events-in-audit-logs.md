---
title: Identificar eliminar eventos de mensagens em registos de auditoria
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 797a4b1146862faf91d2b9e8d74feade90f71650
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716507"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="37407-102">Registos de auditoria para mensagens de e-mail eliminadas</span><span class="sxs-lookup"><span data-stu-id="37407-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="37407-103">A partir de janeiro de 2019, a Microsoft está a ligar a auditoria da caixa de correio por defeito.</span><span class="sxs-lookup"><span data-stu-id="37407-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="37407-104">Caso contrário, para rever apagar eventos de mensagens para um utilizador específico, tem de ativar manualmente as ações de eliminação para auditoria.</span><span class="sxs-lookup"><span data-stu-id="37407-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="37407-105">Se o registo de auditoria da caixa de correio já estiver ativado para a sua organização ou para o utilizador específico, siga os passos abaixo.</span><span class="sxs-lookup"><span data-stu-id="37407-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="37407-106">Inicie sessão no [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="37407-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="37407-107">Clique em **Procurar e Investigar** e selecione Pesquisa de Registo de **Auditoria**.</span><span class="sxs-lookup"><span data-stu-id="37407-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="37407-108">Selecione o intervalo de data sintetiza-se nos campos de data de **início** e data de **fim.**</span><span class="sxs-lookup"><span data-stu-id="37407-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="37407-109">Especifique o nome de utilizador para o utilizador que pretende investigar (o utilizador que apagou os itens).</span><span class="sxs-lookup"><span data-stu-id="37407-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="37407-110">No campo **Atividades,** selecione **Mensagens Eliminadas da pasta De itens Eliminados** e **mensagens movidas para**a pasta De itens Eliminados .</span><span class="sxs-lookup"><span data-stu-id="37407-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="37407-111">Clique em **Procurar**.</span><span class="sxs-lookup"><span data-stu-id="37407-111">Click **Search**.</span></span>

<span data-ttu-id="37407-112">Nos resultados, selecione um registo de auditoria.</span><span class="sxs-lookup"><span data-stu-id="37407-112">In the results, select an audit record.</span></span> <span data-ttu-id="37407-113">Nos detalhes, clique em **Mais Informações.**</span><span class="sxs-lookup"><span data-stu-id="37407-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="37407-114">Informações adicionais sobre o item eliminado (por exemplo, a linha de assunto e a localização do item quando foi eliminado) são apresentadas no campo **AffectedItems.**</span><span class="sxs-lookup"><span data-stu-id="37407-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="37407-115">A propriedade **ClientInfoString** mostrará se a eliminação ocorreu no Outlook, Outlook na web (anteriormente conhecida como Outlook Web App), ou em qualquer outro dispositivo.</span><span class="sxs-lookup"><span data-stu-id="37407-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="37407-116">Para mais informações, consulte [Determinar quem configura o envio de e-mail para uma caixa de correio](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="37407-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="37407-117">**Nota:** Não é possível recuperar itens eliminados utilizando a funcionalidade de registo de auditoria.</span><span class="sxs-lookup"><span data-stu-id="37407-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="37407-118">Para recuperar mensagens eliminadas no Outlook na web, consulte ['Recuperar itens eliminados' na Aplicação Web do Outlook](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="37407-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
