---
title: Regra DLP para número de cartão de crédito que não funciona
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: e2e93bed44749b9017dc6ff919a151d46da7a3fc
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507417"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>Problemas de DLP com números de cartão de crédito

**Importante**: durante estes tempos sem precedentes, estamos a tomar medidas para garantir que os serviços SharePoint Online e OneDrive permaneçam com elevada disponibilidade. Para obter mais informações, visite [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) (Ajustes Temporários de Funcionalidades do SharePoint Online).

**Problemas de DLP com números de cartão de crédito**

Está a ter problemas com **a Prevenção de Perdas de Dados (DLP)** que não está a funcionar para conteúdos que contenham um **Número de Cartão de Crédito** quando utilizar um tipo de informação sensível DLP em O365? Em caso afirmativo, certifique-se de que o seu conteúdo contém as informações necessárias para desencadear a política DLP quando esta for avaliada. Por exemplo, para uma **política de cartão** de crédito configurada com um nível de confiança de 85%, são avaliadas as seguintes e devem ser detetadas para que a regra desencadeie:
  
- **[Formato:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 dígitos que podem ser formatados ou não equipados (ddddddddddddddddddddd) e devem passar no teste luhn.

- **[Padrão:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Um padrão muito complexo e robusto que deteta cartões de todas as grandes marcas em todo o mundo, incluindo Visa, MasterCard, Discover Card, JCB, American Express, cartões oferta e cartões de jantar.

- **[Checkum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Sim, o cheque luhn

- **[Definição:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** Uma política de DLP está 85% confiante de que é detetado este tipo de informação sensível se, dentro de uma proximidade de 300 caracteres:

  - A função Func_credit_card encontra conteúdo que corresponda ao padrão.

  - Um dos seguintes é verdade:

  - Uma palavra-chave de Keyword_cc_verification é encontrada.

  - Uma palavra-chave de Keyword_cc_name é encontrada

  - A função Func_expiration_date encontra uma data no formato de data certa.

  - A parte de verificação passa

    Por exemplo, a seguinte amostra desencadearia uma Política de Números de Cartão de Crédito DLP:

  - Visto: 4485 3647 3952 7352
  
  - Expira: 2/2009

Para obter mais informações sobre o que é necessário para que um **Número de Cartão** de Crédito seja detetado para o seu conteúdo, consulte a seguinte secção neste artigo: [O que os Tipos de Informação Sensível procuram por Cartão de Crédito#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
Utilizando um tipo de informação sensível incorporado diferente, consulte o seguinte artigo para obter informações sobre o que é necessário para outros tipos: [O que os Tipos de Informação Sensível procuram](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  