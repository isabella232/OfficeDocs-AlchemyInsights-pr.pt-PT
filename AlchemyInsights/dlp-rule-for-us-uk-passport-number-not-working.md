---
title: Regra DLP para Número de Passaporte do Reino Unido não funciona
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
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 85e3ed7fdc221981de13ab6e2ada8adf2a3a80b40ff163981e047cc4a02a1514
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004957"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problemas com números de passaportes DLP - Eua/Reino Unido

**Importante**: durante estes tempos sem precedentes, estamos a tomar medidas para garantir que os serviços SharePoint Online e OneDrive permaneçam com elevada disponibilidade. Para obter mais informações, visite [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) (Ajustes Temporários de Funcionalidades do SharePoint Online).

**Problemas de DLP com números de passaportes dos Eua/Reino Unido**

Está a ter problemas com a Prevenção de Perda de Dados **(DLP)** que não funciona em conteúdos que contenham um número de passaporte dos **EUA/Reino** Unido ao utilizar um tipo de informação confidencial DLP no O365? Se for o caso, certifique-se de que o seu conteúdo contém as informações necessárias para aquilo que a política DLP procura quando é avaliada.
  
Por exemplo, para uma política de número de passaporte dos **Eua/Reino** Unido configurada com um nível de confiança de 75%, o seguinte é avaliado e tem de ser detetado para que a regra acione
  
- **[Formato:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Nove dígitos

- **[Padrão:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Nove dígitos consecutivos

- **[Somar Verificação:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Não, não existe Soão Desmarcação

- **[Definição:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** Uma política DLP tem 75% de confiança de que detetou este tipo de informações confidenciais se, dentro de uma proximidade de 300 carateres:

  - A função Func_usa_uk_passport encontra conteúdo que corresponde ao padrão.

  - Foi encontrada uma palavra-chave Keyword_passport a partir do mesmo.

    Por exemplo, a seguinte amostra  aciona a política de número de passaporte dos E.U.A.A.: Número de passaporte 123456789

Para obter mais informações sobre o que é necessário para que um Número de Passaporte dos Eua/Reino Unido seja detetado para o seu conteúdo, consulte a seguinte secção neste artigo: O que os Tipos de Informações Confidenciais parecem para Número de Passaporte do Reino [Unido/Eua](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)
  
Utilizando um tipo de informações confidenciais incorporado diferente, consulte o seguinte artigo para obter informações sobre o que é necessário para outros tipos: O que procuram os Tipos de Informação [Confidenciais](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  