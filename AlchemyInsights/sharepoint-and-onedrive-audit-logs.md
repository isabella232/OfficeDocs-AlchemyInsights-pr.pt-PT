---
title: Relatórios de log de auditoria do SharePoint clássicos
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
ms.openlocfilehash: af5b3c76b82db13bc89c917247e41fa1d8779b68
ms.sourcegitcommit: d5bf97a0bf0547f36b6da9684ce9f16a13a7749e
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/20/2019
ms.locfileid: "37068034"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="28f63-102">Logs de auditoria do SharePoint e do OneDrive</span><span class="sxs-lookup"><span data-stu-id="28f63-102">SharePoint and OneDrive audit logs</span></span>

<span data-ttu-id="28f63-103">**Logs de auditoria unificada moderna do SharePoint e do OneDrive de conformidade**</span><span class="sxs-lookup"><span data-stu-id="28f63-103">**SharePoint and OneDrive Modern Unified Audit logs from compliance**</span></span>

- [<span data-ttu-id="28f63-104">Ativar/desativar o log de auditoria unificada</span><span class="sxs-lookup"><span data-stu-id="28f63-104">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="28f63-105">Nenhuma configuração adicional é necessária no SharePoint ou no OneDrive.</span><span class="sxs-lookup"><span data-stu-id="28f63-105">No additional configuration is required within SharePoint or OneDrive.</span></span>

- <span data-ttu-id="28f63-106">Use a pesquisa de log de auditoria para verificar a atividade dos arquivos, pastas, usuário (s), permissões:</span><span class="sxs-lookup"><span data-stu-id="28f63-106">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

    - [<span data-ttu-id="28f63-107">Atividades de arquivo e página</span><span class="sxs-lookup"><span data-stu-id="28f63-107">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
    - [<span data-ttu-id="28f63-108">Atividades de pasta</span><span class="sxs-lookup"><span data-stu-id="28f63-108">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    - [<span data-ttu-id="28f63-109">Atividades de compartilhamento e solicitação de acesso</span><span class="sxs-lookup"><span data-stu-id="28f63-109">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
    - [<span data-ttu-id="28f63-110">Atividades de sincronização</span><span class="sxs-lookup"><span data-stu-id="28f63-110">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
    - [<span data-ttu-id="28f63-111">Atividades de administração do site</span><span class="sxs-lookup"><span data-stu-id="28f63-111">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)
- <span data-ttu-id="28f63-112">Para obter mais informações sobre como recuperar esses eventos, consulte [Pesquisar o log de auditoria](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="28f63-112">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>

<span data-ttu-id="28f63-113">**Logs de auditoria clássicos do SharePoint**</span><span class="sxs-lookup"><span data-stu-id="28f63-113">**SharePoint classic Audit logs**</span></span>

<span data-ttu-id="28f63-114">Migramos a auditoria de legado do SPO para o Unified Audit Log (UAL).</span><span class="sxs-lookup"><span data-stu-id="28f63-114">We migrated SPO legacy auditing to Unified Audit Log (UAL).</span></span> <span data-ttu-id="28f63-115">Isso significa essencialmente que todos os relatórios de auditoria legados do SPO agora serão movidos por UAL, e os sinais de auditoria herdados foram migrados para o UAL.</span><span class="sxs-lookup"><span data-stu-id="28f63-115">This essentially means that all SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="28f63-116">Principais alterações:</span><span class="sxs-lookup"><span data-stu-id="28f63-116">Key changes:</span></span>

- <span data-ttu-id="28f63-117">Aparar como um recurso não está disponível.</span><span class="sxs-lookup"><span data-stu-id="28f63-117">Trimming as a capability is NOT available.</span></span>
- <span data-ttu-id="28f63-118">A seção onde você escolhe eventos específicos para auditoria não está disponível.</span><span class="sxs-lookup"><span data-stu-id="28f63-118">The section where you choose specific events to audit is NOT available.</span></span> <span data-ttu-id="28f63-119">Refira por favor [este documento](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) para uma lista completa de eventos auditados disponíveis à revelia.</span><span class="sxs-lookup"><span data-stu-id="28f63-119">Please refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
- <span data-ttu-id="28f63-120">A opção "localização" em **relatórios personalizados** não está disponível.</span><span class="sxs-lookup"><span data-stu-id="28f63-120">The "Location" option under **Customized reports** is NOT available.</span></span> 
- <span data-ttu-id="28f63-121">Os eventos "abrindo ou baixando documentos" não estão disponíveis.</span><span class="sxs-lookup"><span data-stu-id="28f63-121">“Opening or downloading documents” events is NOT available.</span></span> 

