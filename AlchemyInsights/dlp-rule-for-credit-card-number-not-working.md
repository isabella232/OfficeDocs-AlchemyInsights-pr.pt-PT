---
title: Regra do DLP para número de cartão de crédito não funcionar
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: a56f32b54e6cb32fa044d26d08868bac8c368de5
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/24/2019
ms.locfileid: "29484589"
---
Está a ter problemas com o **Data Loss Prevention (DLP)** não funcionar para o conteúdo que contenha um **Número de cartão de crédito** quando utilizar um tipo de informações sensíveis do DLP em O365? Se assim for, certifique-se de conteúdo contém as informações necessárias para activar a política DLP quando é avaliado. Por exemplo, para uma **política de cartão de crédito** configurado com um nível de confiança de 85%, a seguir é avaliados e deve ser detectada para a regra accionar: 
  
- **[Formato:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 dígitos que podem ser formatados ou formatada (dddddddddddddddd) e tem de passar no teste de Luhn. 
    
- **[Padrão:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Padrão de muito complexo e robusto que detecta placas de todas as marcas principais em todo o mundo, incluindo Visa, Mastercard, descobrir o cartão, JCB, American Express, cartões de oferta e cartões de diner. 
    
- **[Soma de verificação:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Sim, a soma de verificação de Luhn 
    
- **[Definição:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Uma política DLP é de 85% de certeza de que detectou este tipo de informações sensíveis se, num raio de 300 caracteres: 
    
  - A função Func_credit_card localiza conteúdo que corresponda ao padrão.
    
  - Uma das seguintes afirmações é verdadeira: 
    
  - Foi encontrada uma palavra-chave de Keyword_cc_verification.
    
  - Encontra-se uma palavra-chave de Keyword_cc_name
    
  - A função Func_expiration_date localiza uma data no formato de data à direita.
    
  - As fases de soma de verificação
    
    Por exemplo, o seguinte exemplo daria origem para uma política de número de cartão de crédito do DLP:
    
  - Visto: 4485 3647 3952 7352 
    
  - Expira: 2/2009
    
Para mais informações sobre o que é necessário para um **Número de cartão de crédito** a ser detectado para o seu conteúdo, consulte a secção seguinte deste artigo: [O que o sensíveis a maiúsculas e tipos de informação procure cartão de crédito #](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)
  
Utilizando um tipo de informações sensíveis incorporados diferentes, consulte o artigo seguinte para obter informações sobre o que é necessário para outros tipos: [Procurar o que o sensíveis a maiúsculas e tipos de informação](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

