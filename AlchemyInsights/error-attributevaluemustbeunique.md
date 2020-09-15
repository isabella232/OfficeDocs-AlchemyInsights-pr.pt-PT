---
title: Atributo de erroValueMustBeUnique
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
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 4627a7ae34b0dd9f16538ef75ac8792672dcc056
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709162"
---
# <a name="error-attributevaluemustbeunique"></a>Erro: AtributoValueMustBeUnique

A razão mais comum para o erro AttributeValueMustBeUnique é dois objetos com diferentes SourceAnchor (imuttableId) têm o mesmo valor para os atributos ProxyAddresses e/ou UserPrincipalName. Para corrigir o erro Do ValorValueMustBeUnique:
  
1. Identifique os proxyAddresses duplicados, userPrincipalName ou outro valor de atributo que está a causar o erro. Identifique também quais dois (ou mais) objetos estão envolvidos no conflito. O relatório gerado pela Azure AD Connect Health para sincronização pode ajudá-lo a identificar os dois objetos.
    
2. Identifique qual o objeto que deve continuar a ter o valor duplicado e qual o objeto que não deve.
    
3. Retire o valor duplicado do objeto que NÃO deve ter esse valor. Note que deve fazer a alteração no diretório de onde o objeto é obtido. Em alguns casos, poderá ser necessário eliminar um dos objetos em conflito.
    
4. Se escoda a alteração no AD das instalações, deixe o Azure AD Ligar sincronizar a alteração para que o erro seja corrigido.
    

