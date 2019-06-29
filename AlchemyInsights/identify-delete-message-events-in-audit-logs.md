---
title: Identificar Eliminar mensagem eventos nos registos de auditoria
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 89877331d328d798177fab3150d5219c5b484a70
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/28/2019
ms.locfileid: "35383144"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="683de-102">Registos de auditoria para mensagens de correio electrónico eliminados</span><span class="sxs-lookup"><span data-stu-id="683de-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="683de-103">A partir de Janeiro de 2019, Microsoft é a activação por predefinição o registo de auditoria de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="683de-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="683de-104">Caso contrário, para rever os eventos de mensagem de eliminação de um utilizador específico, tem de activar manualmente as acções de eliminação para auditoria.</span><span class="sxs-lookup"><span data-stu-id="683de-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="683de-105">Se a caixa de correio de auditoria registo já está activado para a sua organização ou para o utilizador específico, siga os passos abaixo.</span><span class="sxs-lookup"><span data-stu-id="683de-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="683de-106">Inicie sessão para o [Centro de conformidade do Office 365 segurança &](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="683de-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="683de-107">Clique em **Procurar e de investigação** e seleccione a **Procura de registo de auditoria**.</span><span class="sxs-lookup"><span data-stu-id="683de-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="683de-108">Seleccione o intervalo de datas nos campos **data de início** e **data de fim** .</span><span class="sxs-lookup"><span data-stu-id="683de-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="683de-109">Especificar o nome de utilizador que pretende investigar (o utilizador que os itens eliminados).</span><span class="sxs-lookup"><span data-stu-id="683de-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="683de-110">No campo **actividades** , seleccione **as mensagens eliminadas da pasta Itens eliminados** e **Moved mensagens para a pasta Itens eliminados**.</span><span class="sxs-lookup"><span data-stu-id="683de-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="683de-111">Clique em **Procurar**.</span><span class="sxs-lookup"><span data-stu-id="683de-111">Click **Search**.</span></span>

<span data-ttu-id="683de-112">Nos resultados, seleccione um registo de auditoria.</span><span class="sxs-lookup"><span data-stu-id="683de-112">In the results, select an audit record.</span></span> <span data-ttu-id="683de-113">Na lista de opções de detalhes, clique em **Mais informações**.</span><span class="sxs-lookup"><span data-stu-id="683de-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="683de-114">Obter informações adicionais sobre a item eliminado (por exemplo, a linha de assunto e a localização do item quando foi eliminado) são apresentadas no campo **AffectedItems** .</span><span class="sxs-lookup"><span data-stu-id="683de-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="683de-115">A propriedade **ClientInfoString** irá mostrar-se a eliminação ocorreu no Outlook, Outlook na web (anteriormente conhecido como o Outlook Web App) ou qualquer outro dispositivo.</span><span class="sxs-lookup"><span data-stu-id="683de-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="683de-116">Para mais informações, consulte [determinar que configurou para uma caixa de correio de reencaminhamento de correio electrónico](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="683de-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="683de-117">**Nota**: não é possível obter itens eliminados utilizando a funcionalidade de registo de auditoria.</span><span class="sxs-lookup"><span data-stu-id="683de-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="683de-118">Para obter mensagens eliminadas no Outlook na web, consulte [recuperar itens no Outlook Web App eliminados](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="683de-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
