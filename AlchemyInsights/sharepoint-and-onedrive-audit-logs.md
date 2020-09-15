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
# <a name="sharepoint-and-onedrive-audit-logs"></a>Registos de auditoria do SharePoint e do OneDrive

## <a name="sharepoint-classic-audit-logs"></a>Registos clássicos de auditoria do SharePoint

A auditoria do legado SPO foi migrada para o Registo de Auditoria Unificado (UAL). Todos os relatórios de auditoria do legado da SPO serão agora alimentados através da UAL, e os sinais de auditoria do legado foram migrados para a UAL.

Alterações de chaves:

* O corte não está disponível como capacidade.
* A escolha de eventos específicos para auditoria não está disponível. Consulte [este documento](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) para obter uma lista completa de eventos auditados disponíveis por padrão.
* A opção **localização** em **relatórios personalizados** NÃO está disponível.
* A opção de eventos **de abertura ou descarregamento de documentos** NÃO está disponível.

[Configurar definições de auditoria para uma recolha de site](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>SharePoint e OneDrive Modern Unified Audit registações de conformidade

* [Ligar/desligar Registo de Auditoria Unificada](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

Não é necessária nenhuma configuração adicional dentro do SharePoint ou oneDrive.

Utilize a pesquisa de registo de auditoria para verificar a atividade dos ficheiros, pastas, user(s), permissões:

* [Atividades de arquivo e página](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [Atividades de pasta](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [Atividades de pedido de partilha e acesso](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [Atividades de sincronização](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [Atividades de administração do site](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

Para obter mais informações sobre como recuperar estes eventos, consulte [procurar o registo de auditoria](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).
