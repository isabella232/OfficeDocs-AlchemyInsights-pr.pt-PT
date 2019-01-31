---
title: Regra do DLP para e.u.a. / número do passaporte Reino Unido não funcionar
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 5722f7b6c9a2f905fed2ef4164787e020260edf7
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/30/2019
ms.locfileid: "29656434"
---
Está a ter problemas com o **Data Loss Prevention (DLP)** não funcionar para que contenha conteúdo uma **dos e.u.a. / número do passaporte UK** quando utilizar um tipo de informações sensíveis do DLP em O365? Nesse caso, certifique-se o conteúdo contém as informações necessárias para que a política do DLP está à procura quando é avaliado. 
  
Por exemplo, para um **dos e.u.a. / número do passaporte UK** política configurada com um nível de confiança de 75%, os seguintes são avaliados e deve ser detectados para a regra accionar 
  
- **[Formato:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nove algarismos 
    
- **[Padrão:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nove algarismos consecutivos. 
    
- **[Soma de verificação:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Não, não existe nenhum soma de verificação 
    
- **[Definição:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** Uma política do DLP corresponde a 75% de certeza de que detectou este tipo de informações sensíveis se, num raio de 300 caracteres: 
    
  - A função Func_usa_uk_passport localiza conteúdo que corresponda ao padrão.
    
  - Foi encontrada uma palavra-chave de Keyword_passport.
    
    Por exemplo, o seguinte exemplo daria origem para o **dos e.u.a. / número do passaporte UK** política: número de Estados Unidos Passport 123456789 
    
Para mais informações sobre o que é necessário para dos e.u.a. / número do passaporte UK para ser detectado para o seu conteúdo, consulte a secção seguinte deste artigo: [localizar o que o sensíveis a maiúsculas e tipos de informação dos e.u.a. / número do passaporte UK](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
Utilizando um tipo de informações sensíveis incorporados diferentes, consulte o artigo seguinte para obter informações sobre o que é necessário para outros tipos: [Procurar o que o sensíveis a maiúsculas e tipos de informação](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

