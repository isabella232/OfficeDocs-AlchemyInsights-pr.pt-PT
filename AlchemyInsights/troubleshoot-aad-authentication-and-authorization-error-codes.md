---
title: Resolução de problemas Códigos de autenticação e autorização Ad Ad (AADSTS)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9800"
- "9005744"
ms.openlocfilehash: 14555dfcb1406fd3a3977012393714a713ff80dc
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037835"
---
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a>Resolução de problemas Códigos de autenticação e autorização Ad Ad (AADSTS)

Para resolver os códigos de erro de autenticação e autorização da AAD (AADSTS), execute os seguintes passos recomendados:

1. **Manusear códigos de erro na sua aplicação**

- A **especificação OAuth2.0** https://tools.ietf.org/html/rfc6749#section-5.2 , fornece orientações sobre como lidar com erros durante a autenticação utilizando a parte de erro da resposta de erro.

    - **erro**: Uma cadeia de código de erro que pode ser usada para classificar tipos de erros que ocorrem e deve ser usado para reagir a erros.
    - O campo **de erro** tem vários valores possíveis - reveja as ligações de documentação do protocolo e as especificações de OAuth 2.0 para obter mais informações sobre erros específicos e como reagir a eles.

- Aqui está uma resposta de erro de amostra:
```
{
  "error": "invalid_scope",
  "error_description": "AADSTS70011: The provided value for the input parameter 'scope' is not 
valid. The scope https://example.contoso.com/activity.read is not valid.\r\nTrace ID: 255d1aef- 8c98-452f-ac51-23d051240864\r\nCorrelation ID: fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7\r\nTimestamp: 2016-01-09 02:02:12Z",
  "error_codes": [
    70011
  ],
  "timestamp": "2016-01-09 02:02:12Z",
  "trace_id": "255d1aef-8c98-452f-ac51-23d051240864",
  "correlation_id": "fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7", 
  "error_uri":"https://login.microsoftonline.com/error?code=70011"
}
```
2. **Procurar informações de código de erro corrente**

- Os códigos de erro e as mensagens estão sujeitos a alterações. Para obter as informações mais atuais, consulte a https://login.microsoftonline.com/error página para encontrar descrições de erros, correções e algumas soluções alternativas sugeridas.
- Também pode pesquisar e resolver códigos de [erro AADSTS listados](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) nos códigos de [autenticação adutor adréia e autorização](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application)do artigo Azure.

3. **Obter ajuda**

- [Opções](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) de apoio e ajuda para programadores - Se precisar de uma resposta para uma pergunta ou ajuda na resolução de um problema não coberto na nossa documentação, talvez seja altura de pedir ajuda a especialistas. Este artigo fornece várias sugestões para obter respostas às suas perguntas à medida que desenvolve aplicações que se integram na plataforma de identidade da Microsoft.








