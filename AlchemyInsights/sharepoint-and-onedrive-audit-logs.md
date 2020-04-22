---
title: Relatórios clássicos de registo de auditoria do SharePoint
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 3270f1ab03bacb235cbdc3d710053c858f0a5183
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741976"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>Registos de auditoria SharePoint e OneDrive

## <a name="sharepoint-classic-audit-logs"></a>Registos de auditoria clássicos do SharePoint

A auditoria do legado SPO foi migrada para o Registo de Auditoria Unificado (UAL). Todos os relatórios de auditoria legado spo serão agora alimentados através da UAL, e os sinais de auditoria legadoforam migrados para a UAL.

Alterações de chave:

* O aparar NÃO está disponível como uma capacidade.
* A escolha de eventos específicos para auditoria NÃO está disponível. Consulte [este documento](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) para obter uma lista completa de eventos auditados disponíveis por padrão.
* A opção **Localização** sob **relatórios personalizados** NÃO está disponível.
* A opção **de abertura ou descarregamento** de documentos não está disponível.

[Configure as definições de auditoria para uma recolha do site](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>SharePoint e OneDrive Modern Unified Audit registos de conformidade

* [Ligar/desligar a exploração de auditoria unificada](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

Não é necessária nenhuma configuração adicional dentro do SharePoint ou do OneDrive.

Utilize a pesquisa de registo de auditoria para verificar a atividade dos ficheiros,pastas ou pastas, user(s), permissões:

* [Atividades de arquivo e página](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [Atividades de pastas](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [Atividades de pedido de partilha e acesso](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [Atividades de sincronização](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [Atividades de administração do site](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

Para obter mais informações sobre como recuperar estes eventos, consulte [o registo de auditoria](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).
