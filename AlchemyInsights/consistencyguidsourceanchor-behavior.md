---
title: ConsistênciaGuid / fonte Comportamento de Origem
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: adac469328485696d1ee1532aa3d6828af0642eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47756294"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistênciaGuid / fonte Comportamento de Origem

O Azure AD Connect (versão 1.1.524.0 e depois) facilita agora a utilização do msDS-ConsistencyGuid como atributo sourceAnchor. Ao utilizar esta função, o Azure AD Connect configura automaticamente as regras de sincronização para:
  
- Utilize o msDS-ConsistencyGuid como o atributo SourceAnchor para objetos do Utilizador. ObjectGUID é utilizado para outros tipos de objetos.
    
- Para qualquer objeto de utilizador AD no local cujo atributo MSDS-ConsistênciayGuid não é povoado, a Azure AD Connect escreve o seu valor objectGUID de volta ao atributo MSDS-ConsistencyGuid no Ative Directory. Após o atributo msDS-ConsistencyGuid ser povoado, a Azure AD Connect exporta o objeto para Azure AD.
    
 **Nota:** Uma vez que um objeto AD no local é importado para Azure AD Connect (isto é, importado para o Espaço de Conector AD e projetado para o Metaverse), não pode mais alterar o seu valor de origemAnchor. Para especificar o valor de origemAnchor para um determinado objeto AD no local, configufique o seu atributo MSDS-ConsistênciayGuid antes de ser importado para Azure AD Connect. 
  
Para obter mais informações sobre SourceAnchor e ConsistencyGuid, consulte o seguinte: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

