---
title: Erro AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 7b98b68fabff6c048f1bab6cf506355114d18658
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/12/2019
ms.locfileid: "29916535"
---
# <a name="error-attributevaluemustbeunique"></a>Erro: AttributeValueMustBeUnique

A razão mais comum para o erro de AttributeValueMustBeUnique é dois objectos com diferente SourceAnchor (immutableId) têm o mesmo valor para os atributos ProxyAddresses e/ou UserPrincipalName. Para corrigir o erro AttributeValueMustBeUnique:
  
1. Identifica o proxyAddresses duplicado, userPrincipalName ou outro valor de atributo que está a causar o erro. Também identifica quais os objectos duas (ou mais) envolvidos no conflito. O relatório gerado pelo Azure AD saúde ligar para sincronização pode ajudar a identificar os dois objectos.
    
2. Identifica qual o objecto deve continuar a ter o valor duplicado e qual o objecto não deve.
    
3. Remova o valor duplicado do objecto que não deve ter esse valor. Tenha em atenção que deve efectuar a alteração no directório onde o objecto é originário de. Em alguns casos, poderá ter de eliminar um dos objectos em conflito.
    
4. Se efectuou a alteração nas instalações nas AD, permitem Azure AD ligar sincronizar a alteração para o erro para obter fixo.
    

