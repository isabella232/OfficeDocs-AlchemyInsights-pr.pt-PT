---
title: ConsistênciaGuid / fonte Comportamento de Origem
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: eafe1ec9636cddc9d73a88beb7ae3ad9f6fad660
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817003"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistênciaGuid / fonte Comportamento de Origem

O Azure AD Connect (versão 1.1.524.0 e depois) facilita agora a utilização do msDS-ConsistencyGuid como atributo sourceAnchor. Ao utilizar esta função, o Azure AD Connect configura automaticamente as regras de sincronização para:
  
- Utilize o msDS-ConsistencyGuid como o atributo SourceAnchor para objetos do Utilizador. ObjectGUID é utilizado para outros tipos de objetos.
    
- Para qualquer objeto de utilizador AD no local cujo atributo MSDS-ConsistênciayGuid não é povoado, a Azure AD Connect escreve o seu valor objectGUID de volta ao atributo MSDS-ConsistencyGuid no Ative Directory. Após o atributo msDS-ConsistencyGuid ser povoado, a Azure AD Connect exporta o objeto para Azure AD.
    
 **Nota:** Uma vez que um objeto AD no local é importado para Azure AD Connect (isto é, importado para o Espaço de Conector AD e projetado para o Metaverse), não pode mais alterar o seu valor de origemAnchor. Para especificar o valor de origemAnchor para um determinado objeto AD no local, configufique o seu atributo MSDS-ConsistênciayGuid antes de ser importado para Azure AD Connect. 
  
Para obter mais informações sobre SourceAnchor e ConsistencyGuid, consulte o seguinte: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

