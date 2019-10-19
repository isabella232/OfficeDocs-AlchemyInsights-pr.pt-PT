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
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 5ac56fa78c66cf3b246bc0cc01f040e27310d629
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/18/2019
ms.locfileid: "36527038"
---
# <a name="error-attributevaluemustbeunique"></a>Erro: AttributeValueMustBeUnique

O motivo mais comum para o erro AttributeValueMustBeUnique é dois objetos com diferentes SourceAnchor (immutableId) têm o mesmo valor para os atributos ProxyAddresses e/ou UserPrincipalName. Para corrigir o erro AttributeValueMustBeUnique:
  
1. Identifique os proxyAddresses duplicados, userPrincipalName ou outro valor de atributo que está causando o erro. Identifique também quais dois (ou mais) objetos estão envolvidos no conflito. O relatório gerado pelo Azure AD Connect Health para sincronização pode ajudá-lo a identificar os dois objetos.
    
2. Identifique qual objeto deve continuar a ter o valor duplicado e qual objeto não deve.
    
3. Remova o valor duplicado do objeto que não deve ter esse valor. Observe que você deve fazer a alteração no diretório onde o objeto é originado. Em alguns casos, talvez seja necessário excluir um dos objetos em conflito.
    
4. Se você fez a alteração no AD local, deixe o Azure AD Connect sincronizar a alteração para que o erro seja corrigido.
    

