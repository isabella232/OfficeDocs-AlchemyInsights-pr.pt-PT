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
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="a1171-102">Comportamento de ConsistênciaGuid / sourceAnchor</span><span class="sxs-lookup"><span data-stu-id="a1171-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="a1171-103">O Azure AD Connect (versão 1.1.524.0 e depois) facilita agora a utilização de msDS-Consistência Como atributo sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="a1171-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="a1171-104">Ao utilizar esta funcionalidade, o Azure AD Connect configura automaticamente as regras de sincronização para:</span><span class="sxs-lookup"><span data-stu-id="a1171-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="a1171-105">Utilize msDS-ConsistênciaGuid como o atributo sourceAnchor para objetos de utilizador.</span><span class="sxs-lookup"><span data-stu-id="a1171-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="a1171-106">O ObjectGUID é utilizado para outros tipos de objetos.</span><span class="sxs-lookup"><span data-stu-id="a1171-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="a1171-107">Para qualquer objeto ad-utilizador no local cujo atributo MSDS-Consistência-Consistência Não é povoado, o Azure AD Connect escreve o seu valor objetivo de volta ao atributo msDS-Consistência-Guia no Diretório Ativo no local.</span><span class="sxs-lookup"><span data-stu-id="a1171-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="a1171-108">Após o atributo MSDS-Consistência-Guid ser povoado, o Azure AD Connect exporta o objeto para AD Azure.</span><span class="sxs-lookup"><span data-stu-id="a1171-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="a1171-109">**Nota:** Uma vez que um objeto AD no local é importado para Azure AD Connect (isto é, importado para o Espaço de Conector AD e projetado para o Metaverse), não pode mais alterar o seu valor de origemAnchor.</span><span class="sxs-lookup"><span data-stu-id="a1171-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="a1171-110">Para especificar o valor sourceAnchor para um determinado objeto AD no local, configure o seu atributo MSDS-Consistência-Guid antes de ser importado para Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="a1171-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="a1171-111">Para obter mais informações sobre SourceAnchor e ConsistênciaGuid, consulte o seguinte: [Azure AD Connect: Conceitos de design](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="a1171-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

