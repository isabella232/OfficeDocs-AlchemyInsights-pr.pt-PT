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
ms.openlocfilehash: cb1b50792b07a1b3b69607bf2f6824141a15922f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32408119"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="6ee72-102">ConsistencyGuid / sourceAnchor comportamento</span><span class="sxs-lookup"><span data-stu-id="6ee72-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="6ee72-103">Ligar de AD Azure (versão 1.1.524.0 e depois) agora facilita a utilização de msDS-ConsistencyGuid como atributo sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="6ee72-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="6ee72-104">Quando utilizar esta funcionalidade, Azure AD ligar configura automaticamente as regras de sincronização para:</span><span class="sxs-lookup"><span data-stu-id="6ee72-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="6ee72-105">Utilize msDS-ConsistencyGuid como o atributo sourceAnchor para objectos de utilizador.</span><span class="sxs-lookup"><span data-stu-id="6ee72-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="6ee72-106">GUID de objecto é utilizado para outros tipos de objecto.</span><span class="sxs-lookup"><span data-stu-id="6ee72-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="6ee72-107">Para qualquer dado locais do utilizador do AD objecto cujo atributo msDS-ConsistencyGuid não estiver preenchidas, Azure escritas AD ligar seu valor objectGUID novamente para o atributo msDS-ConsistencyGuid no local no Active Directory.</span><span class="sxs-lookup"><span data-stu-id="6ee72-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="6ee72-108">Depois do atributo msDS-ConsistencyGuid estiver preenchido, o Azure AD ligar em seguida, exporta o objecto para Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6ee72-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="6ee72-109">**Nota:** Uma vez por um local objecto AD é importado para ligar AD Azure (que é, importado para o espaço de conexão AD e projectado para a Metaverse), não é possível alterar o valor de sourceAnchor já.</span><span class="sxs-lookup"><span data-stu-id="6ee72-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="6ee72-110">Para especificar o valor de sourceAnchor para um dado local AD objecto, configurar o atributo msDS-ConsistencyGuid antes que seja importada para Azure AD ligar.</span><span class="sxs-lookup"><span data-stu-id="6ee72-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="6ee72-111">Para mais informações sobre SourceAnchor e ConsistencyGuid, consulte o seguinte: [Azure AD ligar: conceitos de estrutura](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="6ee72-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

