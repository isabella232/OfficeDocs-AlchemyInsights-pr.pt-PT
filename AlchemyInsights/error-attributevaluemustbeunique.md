---
title: Erro atributoValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 5ac56fa78c66cf3b246bc0cc01f040e27310d629
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/15/2019
ms.locfileid: "36527038"
---
# <a name="error-attributevaluemustbeunique"></a>Erro: AttributeValueMustBeUnique

A razão mais comum para o erro AttributeValueMustBeUnique é dois objetos com SourceAnchor diferente (imutávelId) têm o mesmo valor para os atributos ProxyAddress e/ou UserPrincipalName. Para corrigir o erro AttributeValueMustBeUnique:
  
1. Identifique os proxyAddresses duplicados, o userPrincipalName ou o outro valor de atributo que está causando o erro. Também identificar quais dois (ou mais) objetos estão envolvidos no conflito. O relatório gerado pelo Azure AD Connect Health para sincronização pode ajudá-lo a identificar os dois objetos.
    
2. Identifique qual objeto deve continuar a ter o valor duplicado e qual objeto não deve.
    
3. Remova o valor duplicado do objeto que não deve ter esse valor. Observe que você deve fazer a alteração no diretório de onde o objeto é proveniente. Em alguns casos, você pode precisar excluir um dos objetos em conflito.
    
4. Se você fizer a alteração no Anúncio nas instalações, deixe o Azure AD Connect sincronizar a alteração para que o erro seja corrigido.
    

