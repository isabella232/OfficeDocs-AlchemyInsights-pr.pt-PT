---
title: ConsistencyGuid/sourceAnchor behavior
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
ms.openlocfilehash: 9b5765ff3c59b1312bead41a45a53478a96260df0567f006ab93c3ccfaf4be64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044351"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid/sourceAnchor behavior

O Azure AD Ligação (versão 1.1.524.0 e depois) agora facilita a utilização do msDS-ConsistencyGuid como atributo de origemAnchor. Ao utilizar esta funcionalidade, o Azure AD Ligação configura automaticamente as regras de sincronização para:
  
- Utilize msDS-ConsistencyGuid como o atributo sourceAnchor para objetos User. ObjectGUID é utilizado para outros tipos de objetos.
    
- Para qualquer objeto AD User no local cujo atributo msDS-ConsistencyGuid não seja preenchido, o Azure AD Ligação volta a escrever o valor objectGUID no atributo msDS-ConsistencyGuid no Active Directory no local. Após preencher o atributo msDS-ConsistencyGuid, o Azure AD Ligação em seguida exporta o objeto para o Azure AD.
    
 **Nota:** Assim que um objeto AD no local for importado para o Azure AD Ligação (ou seja, importado para o Espaço do Conector do AD e projetado para o Metaverso), já não pode alterar o valor de origemAnchor. Para especificar o valor de sourceAnchor para um determinado objeto AD no local, configure o atributo msDS-ConsistencyGuid antes de ser importado para o Azure AD Ligação. 
  
Para obter mais informações sobre o SourceAnchor e o ConsistencyGuid, consulte o seguinte: [Azure AD Ligação: Conceitos de estrutura](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

