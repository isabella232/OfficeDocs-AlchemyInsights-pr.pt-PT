---
title: Comportamento de ConsistênciaGuid / sourceAnchor
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: 8527e7c2404742a999041f85ed12d78c48cc0d8c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43705744"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>Comportamento de ConsistênciaGuid / sourceAnchor

O Azure AD Connect (versão 1.1.524.0 e depois) facilita agora a utilização de msDS-Consistência Como atributo sourceAnchor. Ao utilizar esta funcionalidade, o Azure AD Connect configura automaticamente as regras de sincronização para:
  
- Utilize msDS-ConsistênciaGuid como o atributo sourceAnchor para objetos de utilizador. O ObjectGUID é utilizado para outros tipos de objetos.
    
- Para qualquer objeto ad-utilizador no local cujo atributo MSDS-Consistência-Consistência Não é povoado, o Azure AD Connect escreve o seu valor objetivo de volta ao atributo msDS-Consistência-Guia no Diretório Ativo no local. Após o atributo MSDS-Consistência-Guid ser povoado, o Azure AD Connect exporta o objeto para AD Azure.
    
 **Nota:** Uma vez que um objeto AD no local é importado para Azure AD Connect (isto é, importado para o Espaço de Conector AD e projetado para o Metaverse), não pode mais alterar o seu valor de origemAnchor. Para especificar o valor sourceAnchor para um determinado objeto AD no local, configure o seu atributo MSDS-Consistência-Guid antes de ser importado para Azure AD Connect. 
  
Para obter mais informações sobre SourceAnchor e ConsistênciaGuid, consulte o seguinte: [Azure AD Connect: Conceitos de design](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

