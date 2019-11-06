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
# <a name="sharepoint-and-onedrive-audit-logs"></a>Registros de auditoria sharepoint e onedrive

## <a name="sharepoint-classic-audit-logs"></a>Registros clássicos de auditoria sharepoint

A auditoria legada da SPO foi migrada para o Registro Unificado de Auditoria (UAL). Todos os relatórios de auditoria legados da SPO agora serão alimentados através da UAL, e os sinais de auditoria legados foram migrados para a UAL.

Principais mudanças:

* Aparamento não está disponível como uma capacidade.
* A escolha de eventos específicos para auditoria não está disponível. Consulte [este documento](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) para uma lista completa de eventos auditados disponíveis por padrão.
* A opção **de localização** em **relatórios personalizados** não está disponível.
* A opção de eventos de **abertura ou download de documentos** não está disponível.

[Configure as configurações de auditoria para uma coleção de sites](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>Compartilha o Compartilhamento e a Auditoria Unificada Moderna OneDrive registram a conformidade

* [Ativar/desligar a exploração madeireira de auditoria unificada](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

Nenhuma configuração adicional é necessária dentro do SharePoint ou do OneDrive.

Use a pesquisa de registro de auditoria para verificar a atividade do arquivo (s), pasta (s), usuário (s), permissões:

* [Atividades de arquivos e páginas](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [Atividades de pasta](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [Atividades de compartilhamento e solicitação de acesso](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [Atividades de sincronização](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [Atividades de administração do local](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

Para obter mais informações sobre como recuperar esses eventos, [consulte o registro](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)de auditoria.
