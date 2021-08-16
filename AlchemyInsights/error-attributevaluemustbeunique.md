---
title: Error AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 37d6764d19d9cfbb0899a5ab85a4b1530896568adc364122075b7d6f2a32970a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54002131"
---
# <a name="error-attributevaluemustbeunique"></a>Erro: AttributeValueMustBeUnique

O motivo mais comum para o erro AttributeValueMustBeUnique é que dois objetos com SourceAnchor (immutableId) diferentes têm o mesmo valor para os atributos ProxyAddresses e/ou UserPrincipalName. Para corrigir o erro AttributeValueMustBeUnique:
  
1. Identifique os proxyAddresses duplicados, userPrincipalName ou outro valor de atributo que está a causar o erro. Identifique também que dois (ou mais) objetos estão envolvidos no conflito. O relatório gerado pelo Azure AD Ligação Estado de Saúde para sincronização pode ajudá-lo a identificar os dois objetos.
    
2. Identifique que objeto deverá continuar a ter o valor duplicado e qual o objeto que não deve ter.
    
3. Remova o valor duplicado do objeto que NÃO deve ter esse valor. Tenha em atenção que deve fazer a alteração no diretório de origem do objeto. Em alguns casos, poderá ter de eliminar um dos objetos em conflito.
    
4. Se fez a alteração no AD no local, deixe que o Azure AD Ligação sincroniza a alteração para que o erro seja corrigido.
    

