---
title: Relatórios clássicos do registo de auditoria do SharePoint
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
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: daf79f8d75ccdff8ad54f0f307648a5832a6bb71
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662219"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="30ebf-102">Registos de auditoria do SharePoint e do OneDrive</span><span class="sxs-lookup"><span data-stu-id="30ebf-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="30ebf-103">Registos clássicos de auditoria do SharePoint</span><span class="sxs-lookup"><span data-stu-id="30ebf-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="30ebf-104">A auditoria do legado SPO foi migrada para o Registo de Auditoria Unificado (UAL).</span><span class="sxs-lookup"><span data-stu-id="30ebf-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="30ebf-105">Todos os relatórios de auditoria do legado da SPO serão agora alimentados através da UAL, e os sinais de auditoria do legado foram migrados para a UAL.</span><span class="sxs-lookup"><span data-stu-id="30ebf-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="30ebf-106">Alterações de chaves:</span><span class="sxs-lookup"><span data-stu-id="30ebf-106">Key changes:</span></span>

* <span data-ttu-id="30ebf-107">O corte não está disponível como capacidade.</span><span class="sxs-lookup"><span data-stu-id="30ebf-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="30ebf-108">A escolha de eventos específicos para auditoria não está disponível.</span><span class="sxs-lookup"><span data-stu-id="30ebf-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="30ebf-109">Consulte [este documento](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) para obter uma lista completa de eventos auditados disponíveis por padrão.</span><span class="sxs-lookup"><span data-stu-id="30ebf-109">Refer to [this document](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="30ebf-110">A opção **localização** em **relatórios personalizados** NÃO está disponível.</span><span class="sxs-lookup"><span data-stu-id="30ebf-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="30ebf-111">A opção de eventos **de abertura ou descarregamento de documentos** NÃO está disponível.</span><span class="sxs-lookup"><span data-stu-id="30ebf-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="30ebf-112">Configurar definições de auditoria para uma recolha de site</span><span class="sxs-lookup"><span data-stu-id="30ebf-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="30ebf-113">SharePoint e OneDrive Modern Unified Audit registações de conformidade</span><span class="sxs-lookup"><span data-stu-id="30ebf-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="30ebf-114">Ligar/desligar Registo de Auditoria Unificada</span><span class="sxs-lookup"><span data-stu-id="30ebf-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="30ebf-115">Não é necessária nenhuma configuração adicional dentro do SharePoint ou oneDrive.</span><span class="sxs-lookup"><span data-stu-id="30ebf-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="30ebf-116">Utilize a pesquisa de registo de auditoria para verificar a atividade dos ficheiros, pastas, user(s), permissões:</span><span class="sxs-lookup"><span data-stu-id="30ebf-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="30ebf-117">Atividades de arquivo e página</span><span class="sxs-lookup"><span data-stu-id="30ebf-117">File and page activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="30ebf-118">Atividades de pasta</span><span class="sxs-lookup"><span data-stu-id="30ebf-118">Folder activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="30ebf-119">Atividades de pedido de partilha e acesso</span><span class="sxs-lookup"><span data-stu-id="30ebf-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="30ebf-120">Atividades de sincronização</span><span class="sxs-lookup"><span data-stu-id="30ebf-120">Synchronization activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="30ebf-121">Atividades de administração do site</span><span class="sxs-lookup"><span data-stu-id="30ebf-121">Site administration activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="30ebf-122">Para obter mais informações sobre como recuperar estes eventos, consulte [procurar o registo de auditoria](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="30ebf-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
