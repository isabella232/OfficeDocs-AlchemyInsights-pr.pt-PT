---
title: Sincronização de serviços de domínio
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
ms.openlocfilehash: 95b5c3b768caf4b5d80a088a17a33facb39805fc766e4888586ae052d91681e3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057869"
---
# <a name="domain-service-synchronization"></a>Sincronização de serviços de domínio

Os objetos e credenciais num domínio gerido do Azure Active Directory Domain Services (Azure AD DS) podem ser criados localmente no domínio ou sincronizados a partir de um inquilino do Azure Active Directory (Azure AD). Quando implementa o Azure AD DS pela primeira vez, é configurada e iniciada uma sincronização única automática para replicar os objetos a partir do Azure AD. Esta sincronização única continua a ser executada em segundo plano para manter o domínio gerido do Azure AD DS actualizado com quaisquer alterações do Azure AD. Não ocorre sincronização a partir do Azure AD DS de volta para o Azure AD.

Para obter mais detalhes sobre a Azure Active Directory de serviço de domínio, consulte Sincronização de [Serviços de Domínio.](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization) 
