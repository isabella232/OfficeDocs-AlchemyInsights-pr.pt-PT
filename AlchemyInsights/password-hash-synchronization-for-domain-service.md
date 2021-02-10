---
title: Sincronização de hash de palavra-passe para o serviço de domínio
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 7f138837b720926c5b687285a105eb0417ca5b39
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177625"
---
# <a name="password-hash-synchronization-for-domain-service"></a>Sincronização de hash de palavra-passe para o serviço de domínio

**Se a sua instância AD DS Azure estiver a pedir-lhe para ativar a sincronização de hash de palavra-passe**

Encontra-se um cenário em que está a executar um ambiente híbrido com os utilizadores a sincronizar-se a partir de um ambiente no local Azure Ative Directory Domain Services (AD DS). Este cenário encontra-se apesar de ter sincronização de hash de palavra-passe do AD DS no local para o seu inquilino AZure AD.

**Causa**

Isto acontece porque o Azure AD Connect por padrão não sincroniza o legado New Technology LAN Manager (NTLM) e os hashes de password Kerberos que são necessários para o Azure AD DS.

**Solução** 

Você precisaria configurar Azure AD Connect para sincronizar os hashes de palavra-passe necessários para a autenticação NTLM e Kerberos.

Depois de configurado O Azure AD Connect, um evento de criação de conta no local ou de mudança de palavra-passe também sincroniza a palavra-passe do legado hashes para Azure AD. Consulte [aqui](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) mais informações sobre este caso e para obter orientações sobre como permitir a sincronização de passwords em ambientes híbridos Azure AD DS.