---
title: Comportamento de ConsistencyGuid/sourceAnchor
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: f0ff94a8e46f1fb4e0ac8653c51f8f651e29498b
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/18/2019
ms.locfileid: "36517004"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>Comportamento de ConsistencyGuid/sourceAnchor

O Azure AD Connect (versão 1.1.524.0 e depois) agora facilita o uso de msDS-ConsistencyGuid como atributo sourceAnchor. Ao usar esse recurso, o Azure AD Connect configura automaticamente as regras de sincronização para:
  
- Use msDS-ConsistencyGuid como o atributo sourceAnchor para objetos User. ObjectGUID é usado para outros tipos de objeto.
    
- Para qualquer objeto de usuário do AD local fornecido cujo atributo msDS-ConsistencyGuid não é preenchido, o Azure AD Connect grava seu valor objectGUID de volta no atributo msDS-ConsistencyGuid no Active Directory local. Depois que o atributo msDS-ConsistencyGuid é preenchido, o Azure AD Connect, em seguida, exporta o objeto para o Azure AD.
    
 **Nota:** Depois que um objeto AD local é importado para o Azure AD Connect (ou seja, importado para o espaço do conector do AD e projetado para o metaverso), você não pode alterar seu valor sourceAnchor anymore. Para especificar o valor sourceAnchor para um determinado objeto do AD local, configure seu atributo msDS-ConsistencyGuid antes de ser importado para o Azure AD Connect. 
  
Para obter mais informações sobre SourceAnchor e ConsistencyGuid, consulte o seguinte: [Azure ad Connect: conceitos de design](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

