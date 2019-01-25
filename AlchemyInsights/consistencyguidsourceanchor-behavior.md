---
title: ConsistencyGuid / sourceAnchor comportamento
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: 80516ed9e15040475a8b65a1af98a1b561704d49
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/24/2019
ms.locfileid: "29498529"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="f5de6-102">ConsistencyGuid / sourceAnchor comportamento</span><span class="sxs-lookup"><span data-stu-id="f5de6-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="f5de6-p101">Ligar de AD Azure (versão 1.1.524.0 e depois) agora facilita a utilização de msDS-ConsistencyGuid como atributo sourceAnchor. Quando utilizar esta funcionalidade, Azure AD ligar configura automaticamente as regras de sincronização para:</span><span class="sxs-lookup"><span data-stu-id="f5de6-p101">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute. When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="f5de6-p102">Utilize msDS-ConsistencyGuid como o atributo sourceAnchor para objectos de utilizador. GUID de objecto é utilizado para outros tipos de objecto.</span><span class="sxs-lookup"><span data-stu-id="f5de6-p102">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects. ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="f5de6-p103">Para qualquer dado locais do utilizador do AD objecto cujo atributo msDS-ConsistencyGuid não estiver preenchidas, Azure escritas AD ligar seu valor objectGUID novamente para o atributo msDS-ConsistencyGuid no local no Active Directory. Depois do atributo msDS-ConsistencyGuid estiver preenchido, o Azure AD ligar em seguida, exporta o objecto para Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f5de6-p103">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory. After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="f5de6-p104">**Nota:** Uma vez por um local objecto AD é importado para ligar AD Azure (que é, importado para o espaço de conexão AD e projectado para a Metaverse), não é possível alterar o valor de sourceAnchor já. Para especificar o valor de sourceAnchor para um dado local AD objecto, configurar o atributo msDS-ConsistencyGuid antes que seja importada para Azure AD ligar.</span><span class="sxs-lookup"><span data-stu-id="f5de6-p104">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore. To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="f5de6-111">Para mais informações sobre SourceAnchor e ConsistencyGuid, consulte o seguinte: [Azure AD ligar: conceitos de estrutura](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="f5de6-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

