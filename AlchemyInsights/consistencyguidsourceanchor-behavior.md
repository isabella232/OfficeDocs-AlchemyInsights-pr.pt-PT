---
title: ConsistencyGuid / sourceAnchor comportamento
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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36517004"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid / sourceAnchor comportamento

Ligar de AD Azure (versão 1.1.524.0 e depois) agora facilita a utilização de msDS-ConsistencyGuid como atributo sourceAnchor. Quando utilizar esta funcionalidade, Azure AD ligar configura automaticamente as regras de sincronização para:
  
- Utilize msDS-ConsistencyGuid como o atributo sourceAnchor para objectos de utilizador. GUID de objecto é utilizado para outros tipos de objecto.
    
- Para qualquer dado locais do utilizador do AD objecto cujo atributo msDS-ConsistencyGuid não estiver preenchidas, Azure escritas AD ligar seu valor objectGUID novamente para o atributo msDS-ConsistencyGuid no local no Active Directory. Depois do atributo msDS-ConsistencyGuid estiver preenchido, o Azure AD ligar em seguida, exporta o objecto para Azure AD.
    
 **Nota:** Uma vez por um local objecto AD é importado para ligar AD Azure (que é, importado para o espaço de conexão AD e projectado para a Metaverse), não é possível alterar o valor de sourceAnchor já. Para especificar o valor de sourceAnchor para um dado local AD objecto, configurar o atributo msDS-ConsistencyGuid antes que seja importada para Azure AD ligar. 
  
Para mais informações sobre SourceAnchor e ConsistencyGuid, consulte o seguinte: [Azure AD ligar: conceitos de estrutura](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

