---
title: 2609-retenção ou ediscovery-hold
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2609"
- "9000048"
ms.openlocfilehash: 85c41995545efd8e1526d9f7dce4a23929f85be5
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994086"
---
# <a name="unable-to-delete-items-in-sharepoint-online-or-onedrive-for-business"></a>Incapaz de excluir itens no SharePoint Online ou OneDrive for Business

Você ou seus usuários podem não poder excluir itens no SharePoint Online ou no OneDrive for Business porque uma política de retenção, rótulo de retenção ou retenção de eDiscovery é aplicada a um site Do Ponto de Compartilhamento do OneDrive ou a um item específico. Isso inclui ser incapaz de excluir um documento, uma versão de documento, uma pasta, uma biblioteca de documentos, uma lista, um aplicativo, um site ou uma coleção de sites. Aqui estão alguns exemplos das mensagens de erro que você pode receber se você tentar excluir um item que está sendo mantido:

- "Este site não pode ser excluído porque está incluído em uma política de retenção ou retenção do eDiscovery"
- "Este site tem uma política de conformidade definida para bloquear a exclusão"
- "Uma política de conformidade está bloqueando essa exclusão do site"
- "Esta coleção do site não pode ser excluída porque contém sites que estão incluídos em uma política de retenção ou retenção do eDiscovery"
- "Você tem que excluir todos os itens nesta pasta antes de excluir a pasta"
- "As versões deste item não podem ser excluídas porque ele está em espera ou na política de retenção"
- "Item não pode ser excluído enquanto estiver em espera"
- "O rótulo que é aplicado a este item impede que ele seja editado ou excluído"
- "A lista não pode ser excluída enquanto estiver em espera ou na política de retenção"
- "A lista não pode ser excluída se for bloqueada ou se uma política de retenção for aplicada a ela"

Para excluir itens em um desses cenários, a política de retenção, o rótulo de retenção ou a retenção do eDiscovery precisa ser removido (ou um site precisa ser excluído de uma política de retenção). Você precisa desativar ou excluir a respectiva espera que está causando esse problema. Depois que uma política ou uma retenção de retenção forem removidas, pode levar até 24 horas para que a alteração entre em vigor. 

Para obter informações sobre os diferentes recursos de retenção e retenção que podem ser aplicados em sites do SharePoint e contas OneDrive, consulte um dos seguintes tópicos.

- [Visão geral das políticas de retenção](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)

- [Visão geral dos rótulos de retenção](https://docs.microsoft.com/microsoft-365/compliance/labels)

- [Gerenciar detém em advanced eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/managing-holds)

- [eDiscovery detém](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-cases#step-4-place-content-locations-on-hold)

- [Políticas de fechamento e exclusão de sites legados](https://support.office.com/article/Use-policies-for-site-closure-and-deletion-A8280D82-27FD-48C5-9ADF-8A5431208BA5)
