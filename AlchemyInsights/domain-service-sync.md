---
title: Sincronização do serviço de domínio
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003245"
- "7922"
- "7921"
ms.openlocfilehash: b35d3a402bc08a27a818209385c5666b901fa524
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885567"
---
# <a name="domain-service-synchronization"></a>Sincronização do serviço de domínio

Objetos e credenciais num domínio gerido por Azure Ative Directory Domain Services (Azure AD DS) podem ser criados localmente dentro do domínio, ou sincronizados a partir de um inquilino do Azure Ative Directory (Azure AD). Quando implementa pela primeira vez O AD DS, uma sincronização automática de sentido único é configurada e iniciada para replicar os objetos do Azure AD. Esta sincronização unidirecionais continua a ser executada em segundo plano para manter o domínio gerido Azure AD DS atualizado com quaisquer alterações a partir de Azure AD. Não ocorre sincronização desde Azure AD DS até Azure AD.

Para obter mais detalhes sobre a sincronização do serviço de domínio do Azure Ative Directory, consulte [a Sincronização do Serviço de Domínio](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization). 
