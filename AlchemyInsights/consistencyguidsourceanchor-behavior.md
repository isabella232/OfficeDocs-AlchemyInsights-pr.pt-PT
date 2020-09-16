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
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="8781f-102">ConsistênciaGuid / fonte Comportamento de Origem</span><span class="sxs-lookup"><span data-stu-id="8781f-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="8781f-103">O Azure AD Connect (versão 1.1.524.0 e depois) facilita agora a utilização do msDS-ConsistencyGuid como atributo sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="8781f-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="8781f-104">Ao utilizar esta função, o Azure AD Connect configura automaticamente as regras de sincronização para:</span><span class="sxs-lookup"><span data-stu-id="8781f-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="8781f-105">Utilize o msDS-ConsistencyGuid como o atributo SourceAnchor para objetos do Utilizador.</span><span class="sxs-lookup"><span data-stu-id="8781f-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="8781f-106">ObjectGUID é utilizado para outros tipos de objetos.</span><span class="sxs-lookup"><span data-stu-id="8781f-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="8781f-107">Para qualquer objeto de utilizador AD no local cujo atributo MSDS-ConsistênciayGuid não é povoado, a Azure AD Connect escreve o seu valor objectGUID de volta ao atributo MSDS-ConsistencyGuid no Ative Directory.</span><span class="sxs-lookup"><span data-stu-id="8781f-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="8781f-108">Após o atributo msDS-ConsistencyGuid ser povoado, a Azure AD Connect exporta o objeto para Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8781f-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="8781f-109">**Nota:** Uma vez que um objeto AD no local é importado para Azure AD Connect (isto é, importado para o Espaço de Conector AD e projetado para o Metaverse), não pode mais alterar o seu valor de origemAnchor.</span><span class="sxs-lookup"><span data-stu-id="8781f-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="8781f-110">Para especificar o valor de origemAnchor para um determinado objeto AD no local, configufique o seu atributo MSDS-ConsistênciayGuid antes de ser importado para Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="8781f-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="8781f-111">Para obter mais informações sobre SourceAnchor e ConsistencyGuid, consulte o seguinte: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="8781f-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

