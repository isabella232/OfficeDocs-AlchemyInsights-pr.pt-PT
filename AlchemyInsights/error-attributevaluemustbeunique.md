---
title: Error AttributeValueMustBeUnique
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
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: fa1fdb35f1af250bc98aa61c0e5111f1f1b8aac4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703185"
---
# <a name="error-attributevaluemustbeunique"></a>Erro: AttributeValueMustBeUnique

A razão mais comum para o erro AttributeValueMustBeUnique é dois objetos com fontediferente (imutávelId) têm o mesmo valor para os atributos ProxyAddresss e/ou UserPrincipalName. Para corrigir o erro AttributeValueMustBeUnique:
  
1. Identifique os proxyAddresses duplicados, userPrincipalName ou outro valor de atributo que está a causar o erro. Identifique também quais dois (ou mais) objetos estão envolvidos no conflito. O relatório gerado pela Azure AD Connect Health para sincronização pode ajudá-lo a identificar os dois objetos.
    
2. Identifique qual o objeto que deve continuar a ter o valor duplicado e qual o objeto que não deve.
    
3. Retire o valor duplicado do objeto que NÃO deve ter esse valor. Note que deve fazer a alteração no diretório de onde o objeto é proveniente. Em alguns casos, poderá ser necessário apagar um dos objetos em conflito.
    
4. Se tiver feito a alteração no ad-local, deixe o Azure AD Connect sincronizar a alteração para que o erro seja corrigido.
    

