---
title: Regra DLP para o Número da Conta Bancária dos EUA que não está a funcionar
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
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: d19b2dcc29e23fab522159945496165338a117a47bfcfcadf0b93e4e5f14464f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005029"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>Problemas de DLP com números de conta bancária dos EUA

**Importante**: durante estes tempos sem precedentes, estamos a tomar medidas para garantir que os serviços SharePoint Online e OneDrive permaneçam com elevada disponibilidade. Para obter mais informações, visite [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) (Ajustes Temporários de Funcionalidades do SharePoint Online).

**Problemas de DLP com números de conta bancária dos EUA**

Está **a** ter problemas com a Prevenção de Perda de Dados **(DLP)** que não funciona em conteúdos que contenham um Número de Conta Bancária dos EUA ao utilizar um tipo de informação confidencial DLP no O365? Se for o caso, certifique-se de que o seu conteúdo contém as informações necessárias para aquilo que a política DLP procura quando é avaliada.
  
Por exemplo, para uma política de Número de Conta Bancária dos EUA configurada com um nível de confiança de 85%, o seguinte é avaliado e tem de ser detetado para que **a** regra acione:
  
- **[Formato:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8 a 17 dígitos

- **[Padrão:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8 a 17 dígitos consecutivos.

- **[Somar Verificação:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Não, não existe Soão Desmarcação

- **[Definição:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** Uma política DLP tem 75% de confiança de que detetou este tipo de informações confidenciais se, dentro de uma proximidade de 300 carateres:

  - A expressão Regex_usa_bank_account_number encontra conteúdo que corresponde ao padrão

  - Foi encontrada uma palavra-Keyword_usa_Bank_Account a partir do mesmo.

    Por exemplo, a seguinte amostra seria ativada para a política Número de Conta **Bancária** dos EUA: Verificar Conta 78344011

Para obter mais informações sobre o que é necessário para **que** um Número de Conta Bancária dos EUA seja detetado no seu conteúdo, consulte a seguinte secção neste artigo: O que os Tipos de Informações Confidenciais procuram para o Número da Conta Bancária dos [EUA](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)
  
Utilizando um tipo de informações confidenciais incorporado diferente, consulte o seguinte artigo para obter informações sobre o que é necessário para outros tipos: O que procuram os Tipos de Informação [Confidenciais](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  