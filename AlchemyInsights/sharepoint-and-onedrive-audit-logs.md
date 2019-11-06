---
title: Relatórios clássicos de registro de auditoria sharepoint
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: be95034bea3c58a4fde96cfb0f9ba525e810758e
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/05/2019
ms.locfileid: "37992629"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="f9035-102">Registros de auditoria sharepoint e onedrive</span><span class="sxs-lookup"><span data-stu-id="f9035-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="f9035-103">Registros clássicos de auditoria sharepoint</span><span class="sxs-lookup"><span data-stu-id="f9035-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="f9035-104">A auditoria legada da SPO foi migrada para o Registro Unificado de Auditoria (UAL).</span><span class="sxs-lookup"><span data-stu-id="f9035-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="f9035-105">Todos os relatórios de auditoria legados da SPO agora serão alimentados através da UAL, e os sinais de auditoria legados foram migrados para a UAL.</span><span class="sxs-lookup"><span data-stu-id="f9035-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="f9035-106">Principais mudanças:</span><span class="sxs-lookup"><span data-stu-id="f9035-106">Key changes:</span></span>

* <span data-ttu-id="f9035-107">Aparamento não está disponível como uma capacidade.</span><span class="sxs-lookup"><span data-stu-id="f9035-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="f9035-108">A escolha de eventos específicos para auditoria não está disponível.</span><span class="sxs-lookup"><span data-stu-id="f9035-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="f9035-109">Consulte [este documento](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) para uma lista completa de eventos auditados disponíveis por padrão.</span><span class="sxs-lookup"><span data-stu-id="f9035-109">Refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="f9035-110">A opção **de localização** em **relatórios personalizados** não está disponível.</span><span class="sxs-lookup"><span data-stu-id="f9035-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="f9035-111">A opção de eventos de **abertura ou download de documentos** não está disponível.</span><span class="sxs-lookup"><span data-stu-id="f9035-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="f9035-112">Configure as configurações de auditoria para uma coleção de sites</span><span class="sxs-lookup"><span data-stu-id="f9035-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="f9035-113">Compartilha o Compartilhamento e a Auditoria Unificada Moderna OneDrive registram a conformidade</span><span class="sxs-lookup"><span data-stu-id="f9035-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="f9035-114">Ativar/desligar a exploração madeireira de auditoria unificada</span><span class="sxs-lookup"><span data-stu-id="f9035-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="f9035-115">Nenhuma configuração adicional é necessária dentro do SharePoint ou do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="f9035-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="f9035-116">Use a pesquisa de registro de auditoria para verificar a atividade do arquivo (s), pasta (s), usuário (s), permissões:</span><span class="sxs-lookup"><span data-stu-id="f9035-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="f9035-117">Atividades de arquivos e páginas</span><span class="sxs-lookup"><span data-stu-id="f9035-117">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="f9035-118">Atividades de pasta</span><span class="sxs-lookup"><span data-stu-id="f9035-118">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="f9035-119">Atividades de compartilhamento e solicitação de acesso</span><span class="sxs-lookup"><span data-stu-id="f9035-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="f9035-120">Atividades de sincronização</span><span class="sxs-lookup"><span data-stu-id="f9035-120">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="f9035-121">Atividades de administração do local</span><span class="sxs-lookup"><span data-stu-id="f9035-121">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="f9035-122">Para obter mais informações sobre como recuperar esses eventos, [consulte o registro](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)de auditoria.</span><span class="sxs-lookup"><span data-stu-id="f9035-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
