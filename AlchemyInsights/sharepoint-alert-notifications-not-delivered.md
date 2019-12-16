---
title: Notificações de alerta sharepoint não entregues
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: 978ca8df40736228932ae6f6a7c33ad0b159d4e5
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40047078"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a><span data-ttu-id="b0f2f-102">Notificações de alerta sharepoint não entregues</span><span class="sxs-lookup"><span data-stu-id="b0f2f-102">SharePoint alert notifications not delivered</span></span>

<span data-ttu-id="b0f2f-103">Por favor, verifique a pasta JUNK em seu e-mail, como às vezes alertas podem ir lá.</span><span class="sxs-lookup"><span data-stu-id="b0f2f-103">Please check the JUNK folder in your email, as sometimes alerts might go there.</span></span>

<span data-ttu-id="b0f2f-104">Determinar se **todos os alertas não são entregues** ou se um alerta **individual** de um arquivo ou biblioteca específico não é entregue.</span><span class="sxs-lookup"><span data-stu-id="b0f2f-104">Determine if **all alerts are not delivered** or if **an individual alert** from a specific file or library is not delivered.</span></span>

- <span data-ttu-id="b0f2f-105">**Os alertas individuais não são entregues:** se um alerta individual de um arquivo ou biblioteca específico não for entregue, você pode tentar excluí-lo e recriá-lo.</span><span class="sxs-lookup"><span data-stu-id="b0f2f-105">**Individual alerts are not delivered**: If an individual alert from a specific file or library is not delivered, you can attempt to delete and recreate it.</span></span> <span data-ttu-id="b0f2f-106">Veja [gerenciar, visualizar ou excluir os alertas do SharePoint](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2?ui=en-US&rs=&ad=US#ID0EAADAAA=Online) para recriar o alerta.</span><span class="sxs-lookup"><span data-stu-id="b0f2f-106">See [Manage, view, or delete SharePoint alerts](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2?ui=en-US&rs=&ad=US#ID0EAADAAA=Online) to recreate the alert.</span></span>
- <span data-ttu-id="b0f2f-107">**Todos os alertas não são entregues:** Se todos os alertas de vários arquivos ou bibliotecas não forem entregues, visite o painel de Saúde do [Serviço](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) para verificar se há avisos/incidentes que possam estar ocorrendo com o SharePoint ou o Exchange.</span><span class="sxs-lookup"><span data-stu-id="b0f2f-107">**All alerts are not delivered**: If all alerts from multiple files or libraries are not delivered, visit the [Service Health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="b0f2f-108">O problema pode ser com a capacidade de alerta SharePoint ou atrasos nos e-mails através da Troca.</span><span class="sxs-lookup"><span data-stu-id="b0f2f-108">The issue could be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="b0f2f-109">Também será importante notar se outros e-mails estão sendo entregues e, se não, o problema é provável com atrasos de câmbio.</span><span class="sxs-lookup"><span data-stu-id="b0f2f-109">It will also be important to note whether other email is being delivered, and if not, the issue is likely with Exchange delays.</span></span>

<span data-ttu-id="b0f2f-110">FAQ em alertas:</span><span class="sxs-lookup"><span data-stu-id="b0f2f-110">FAQ on alerts:</span></span>

- <span data-ttu-id="b0f2f-111">Não é possível enviar alertas para o Grupo de Distribuição, apenas os grupos Security e O365 são apoiados.</span><span class="sxs-lookup"><span data-stu-id="b0f2f-111">It is not possible to send alerts to Distribution Group, only Security and O365 groups are supported.</span></span>
- <span data-ttu-id="b0f2f-112">Você não pode personalizar modelos de e-mail de alerta; você precisa usar o Microsoft FLOW ou o SharePoint Designer Workflow para alcançá-los.</span><span class="sxs-lookup"><span data-stu-id="b0f2f-112">You cannot customize alert email templates; you need to use Microsoft FLOW or SharePoint Designer Workflow to achieve those.</span></span>

<span data-ttu-id="b0f2f-113">Mais informações:</span><span class="sxs-lookup"><span data-stu-id="b0f2f-113">More Information:</span></span>

- <span data-ttu-id="b0f2f-114">**Configuração**de alerta: Para obter mais informações sobre a configuração de alertas, [consulte criar um alerta para ser notificado quando um arquivo ou pasta mudar no SharePoint](https://support.office.com/article/create-an-alert-to-get-notified-when-a-file-or-folder-changes-in-sharepoint-e5a79e7b-a146-46da-a9ef-d65409ba8918).</span><span class="sxs-lookup"><span data-stu-id="b0f2f-114">**Alert setup**: For more information about setting up alerts, see [Create an alert to get notified when a file or folder changes in SharePoint](https://support.office.com/article/create-an-alert-to-get-notified-when-a-file-or-folder-changes-in-sharepoint-e5a79e7b-a146-46da-a9ef-d65409ba8918).</span></span>
- <span data-ttu-id="b0f2f-115">**Alertas de solucionamento de problemas:** Para obter mais informações sobre alertas de solução de problemas, consulte [os usuários não recebam notificações de alerta on-line do SharePoint.](https://docs.microsoft.com/sharepoint/support/sites/no-alert-notifications)</span><span class="sxs-lookup"><span data-stu-id="b0f2f-115">**Troubleshoot alerts**: For more information about troubleshooting alerts, see [Users don't receive SharePoint Online alert notifications](https://docs.microsoft.com/sharepoint/support/sites/no-alert-notifications).</span></span>
- <span data-ttu-id="b0f2f-116">Políticas avançadas de alerta de **conformidade o365:** para obter mais informações sobre a configuração desses alertas, consulte [as Políticas](https://docs.microsoft.com/office365/securitycompliance/alert-policies)de Alerta de Conformidade.</span><span class="sxs-lookup"><span data-stu-id="b0f2f-116">**Advanced O365 Compliance Alert Policies**: For more information about setting up these alerts, see [Compliance Alert Policies](https://docs.microsoft.com/office365/securitycompliance/alert-policies).</span></span>
- <span data-ttu-id="b0f2f-117">Registros de **auditoria sharepoint e onedrive:** para obter mais informações sobre como recuperar esses eventos, [consulte o registro](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)de auditoria .</span><span class="sxs-lookup"><span data-stu-id="b0f2f-117">**SharePoint and OneDrive Audit Logs**: For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
- <span data-ttu-id="b0f2f-118">**Alertas enviados pela Proteção avançada de ameaças:** Veja [ATP para SharePoint e OneDrive](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="b0f2f-118">**Alerts sent by Advanced Threat Protection**: See [ATP for SharePoint and OneDrive](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>
- <span data-ttu-id="b0f2f-119">**Alertas enviados pelas políticas**de Prevenção de Perdas de Dados: Veja notificações por [e-mail para as políticas](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)de DLP .</span><span class="sxs-lookup"><span data-stu-id="b0f2f-119">**Alerts sent by Data Loss Prevention polices**: See [Email notifications for DLP policies](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span></span>

## <a name="related-topics"></a><span data-ttu-id="b0f2f-120">Tópicos relacionados</span><span class="sxs-lookup"><span data-stu-id="b0f2f-120">Related Topics</span></span>

<span data-ttu-id="b0f2f-121">Quer experimentar o Microsoft Flow no SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="b0f2f-121">Want to try Microsoft Flow in SharePoint Online?</span></span>

- [<span data-ttu-id="b0f2f-122">Criar fluxo</span><span class="sxs-lookup"><span data-stu-id="b0f2f-122">Create Flow</span></span>](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [<span data-ttu-id="b0f2f-123">SharePoint e Flow</span><span class="sxs-lookup"><span data-stu-id="b0f2f-123">SharePoint and Flow</span></span>](https://flow.microsoft.com//blog/sharepoint-and-flow/)
