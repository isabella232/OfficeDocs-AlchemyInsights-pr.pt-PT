---
title: Regra dLP para número de cartão de crédito não funcionando
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 6b28534d072c024a98a9b05f6cb55bfdc3435db6
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932454"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>DLP emite com números de cartão de crédito

**Importante**: Muitos clientes SharePoint Online e OneDrive executam aplicações críticas ao negócio contra o serviço que executa em segundo plano. Estes incluem migração de conteúdos, Prevenção de Perdas de Dados (DLP) e soluções de backup. Durante estes tempos sem precedentes, estamos a tomar medidas para garantir que os serviços SharePoint Online e OneDrive permanecem altamente disponíveis e fiáveis para os seus utilizadores que dependem mais do serviço do que nunca em cenários de trabalho remoto.

Em apoio a este objetivo, implementámos limites de estrangulamento mais apertados em aplicações de fundo (soluções de migração, DLP e backup) durante o dia da semana. Deve esperar que estas aplicações atinjam uma entrada muito limitada durante estes tempos. No entanto, durante as horas de noite e fim de semana para a região, o serviço estará pronto para processar um volume significativamente maior de pedidos de aplicações de fundo.

**DLP emite com números de cartão de crédito**

Está a ter problemas com a Prevenção de Perdas de **Dados (DLP)** que não está a trabalhar para conteúdos que contenham um Número de **Cartão** de Crédito ao utilizar um tipo de informação sensível dLP em O365? Em caso afirmativo, certifique-se de que o seu conteúdo contém as informações necessárias para desencadear a política dLP quando for avaliada. Por exemplo, para uma política de **Cartão** de Crédito configurada com um nível de confiança de 85%, são avaliados e devem ser detetados para que a regra desencadeie:
  
- **[Formato:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 dígitos que podem ser formatados ou não formatados (ddddddddddddddddddddddddddddd) e devem passar no teste Luhn.

- **[Padrão:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Padrão muito complexo e robusto que deteta cartões de todas as grandes marcas em todo o mundo, incluindo Visa, MasterCard, Discover Card, JCB, American Express, cartões oferta e cartões de jantar.

- **[Chequeum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Sim, o cheque Luhn.

- **[Definição:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Uma política de DLP está 85% confiante de que detetou este tipo de informação sensível se, dentro de uma proximidade de 300 caracteres:

  - A função Func_credit_card encontra conteúdo que corresponda ao padrão.

  - Um dos seguintes é verdade:

  - Uma palavra-chave de Keyword_cc_verification é encontrada.

  - Uma palavra-chave de Keyword_cc_name é encontrada

  - A função Func_expiration_date encontra uma data no formato de data certa.

  - O cheque passa

    Por exemplo, a seguinte amostra desencadearia uma Política de Números de Cartão de Crédito DLP:

  - Visto: 4485 3647 3952 7352
  
  - Expira: 2/2009

Para obter mais informações sobre o que é necessário para que um Número de **Cartão** de Crédito seja detetado para o seu conteúdo, consulte a seguinte secção neste artigo: [O que os Tipos de Informação Sensível procuram para cartão](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number) de crédito#
  
Utilizando um tipo de informação sensível incorporado diferente, consulte o seguinte artigo para obter informações sobre o que é necessário para outros tipos: O que os Tipos de [Informação Sensível procuram](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  