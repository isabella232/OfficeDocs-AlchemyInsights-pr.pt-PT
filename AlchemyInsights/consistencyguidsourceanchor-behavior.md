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
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="8b28e-102">Comportamento de ConsistencyGuid/sourceAnchor</span><span class="sxs-lookup"><span data-stu-id="8b28e-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="8b28e-103">O Azure AD Connect (versão 1.1.524.0 e depois) agora facilita o uso de msDS-ConsistencyGuid como atributo sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="8b28e-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="8b28e-104">Ao usar esse recurso, o Azure AD Connect configura automaticamente as regras de sincronização para:</span><span class="sxs-lookup"><span data-stu-id="8b28e-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="8b28e-105">Use msDS-ConsistencyGuid como o atributo sourceAnchor para objetos User.</span><span class="sxs-lookup"><span data-stu-id="8b28e-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="8b28e-106">ObjectGUID é usado para outros tipos de objeto.</span><span class="sxs-lookup"><span data-stu-id="8b28e-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="8b28e-107">Para qualquer objeto de usuário do AD local fornecido cujo atributo msDS-ConsistencyGuid não é preenchido, o Azure AD Connect grava seu valor objectGUID de volta no atributo msDS-ConsistencyGuid no Active Directory local.</span><span class="sxs-lookup"><span data-stu-id="8b28e-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="8b28e-108">Depois que o atributo msDS-ConsistencyGuid é preenchido, o Azure AD Connect, em seguida, exporta o objeto para o Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8b28e-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="8b28e-109">**Nota:** Depois que um objeto AD local é importado para o Azure AD Connect (ou seja, importado para o espaço do conector do AD e projetado para o metaverso), você não pode alterar seu valor sourceAnchor anymore.</span><span class="sxs-lookup"><span data-stu-id="8b28e-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="8b28e-110">Para especificar o valor sourceAnchor para um determinado objeto do AD local, configure seu atributo msDS-ConsistencyGuid antes de ser importado para o Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="8b28e-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="8b28e-111">Para obter mais informações sobre SourceAnchor e ConsistencyGuid, consulte o seguinte: [Azure ad Connect: conceitos de design](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="8b28e-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

