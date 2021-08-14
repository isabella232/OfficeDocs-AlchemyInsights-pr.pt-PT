---
title: Regra DLP para o Número de Cartão de Crédito que não funciona
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: bd4f200233d5571fc7b01576038e7b3951a07716a7d5948005418d2896291ee5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005101"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>Problemas de DLP com números de cartão de crédito

**Importante**: durante estes tempos sem precedentes, estamos a tomar medidas para garantir que os serviços SharePoint Online e OneDrive permaneçam com elevada disponibilidade. Para obter mais informações, visite [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) (Ajustes Temporários de Funcionalidades do SharePoint Online).

**Problemas de DLP com números de cartão de crédito**

Está **a** ter problemas com a Prevenção de Perda de Dados **(DLP)** que não funciona em conteúdos que contenham um Número de Cartão de Crédito ao utilizar um tipo de informação confidencial DLP no O365? Se for o caso, certifique-se de que o seu conteúdo contém as informações necessárias para ativar a política DLP quando for avaliada. Por exemplo, para uma política de Cartão de Crédito configurada com um nível de confiança de 85%, são avaliados o seguinte e tem de ser detetado para que **a** regra acione:
  
- **[Formato:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 dígitos que podem ser formatados ou não formatados (ddddddddd) e que têm de passar no teste de Luhn.

- **[Padrão:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Padrão muito complexo e robusto que deteta cartões de todas as principais marcas em todo o mundo, incluindo o Visa, MasterCard, Discover Card, JCB, American Express, cartões de oferta e cartões de diner.

- **[Somar Verificação:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Sim, a somar de verificação Luhn

- **[Definição:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** Uma política DLP tem 85% de confiança de que detetou este tipo de informações confidenciais se, dentro de uma proximidade de 300 carateres:

  - A Func_credit_card encontra conteúdo que corresponde ao padrão.

  - Uma das seguintes coisas é verdadeira:

  - Foi encontrada uma palavra-chave Keyword_cc_verification a partir do mesmo.

  - Foi encontrada uma palavra-Keyword_cc_name-chave

  - A Func_expiration_date encontra uma data no formato de data certo.

  - A somar de verificação é ultrapassada

    Por exemplo, a seguinte amostra aciona uma Política de Número de Cartão de Crédito DLP:

  - Visa: 4485 3647 3952 7352
  
  - Expira: 2/2009

Para obter mais informações sobre o que é necessário para **que** um Número de Cartão de Crédito seja detetado para o seu conteúdo, consulte a seguinte secção neste artigo: O que os Tipos de Informações Confidenciais procuram Cartão de [Crédito#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
Utilizando um tipo de informações confidenciais incorporado diferente, consulte o seguinte artigo para obter informações sobre o que é necessário para outros tipos: O que procuram os Tipos de Informação [Confidenciais](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  