---
title: Regra DLP para número de passaporte dos EUA/Reino Unido que não funcione
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 3d3b7dc2d9510376bc9eef6ec69b87ad7c681b05
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507309"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problemas com números de passaportes DLP - EUA/Reino Unido

**Importante**: durante estes tempos sem precedentes, estamos a tomar medidas para garantir que os serviços SharePoint Online e OneDrive permaneçam com elevada disponibilidade. Para obter mais informações, visite [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) (Ajustes Temporários de Funcionalidades do SharePoint Online).

**Problemas de DLP com números de passaportes EUA/Reino Unido**

Está a ter problemas com **a Prevenção de Perdas de Dados (DLP)** que não está a trabalhar para conteúdos que contenham um **número de passaporte dos EUA/Reino Unido** quando utilizar um tipo de informação sensível DLP em O365? Em caso afirmativo, certifique-se de que o seu conteúdo contém as informações necessárias para o que a política de DLP procura quando é avaliada.
  
Por exemplo, para uma política **de número de passaportes dos EUA/Reino Unido** configurada com um nível de confiança de 75%, são avaliadas as seguintes e devem ser detetadas para que a regra desencadeie
  
- **[Formato:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Nove dígitos

- **[Padrão:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Nove dígitos consecutivos

- **[Checkum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Não, não há Cheques.

- **[Definição:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** Uma política de DLP está 75% confiante de que é detetado este tipo de informação sensível se, dentro de uma proximidade de 300 caracteres:

  - A função Func_usa_uk_passport encontra conteúdo que corresponda ao padrão.

  - Uma palavra-chave de Keyword_passport é encontrada.

    Por exemplo, a seguinte amostra desencadearia a política de **número de passaportes dos EUA/Reino Unido:** Número de passaporte dos EUA 123456789

Para obter mais informações sobre o que é necessário para que um número de passaporte dos EUA/Reino Unido seja detetado para o seu conteúdo, consulte a seguinte secção neste artigo: [O que os tipos de informação sensível procuram para o número de passaporte dos EUA/Reino Unido](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)
  
Utilizando um tipo de informação sensível incorporado diferente, consulte o seguinte artigo para obter informações sobre o que é necessário para outros tipos: [O que os Tipos de Informação Sensível procuram](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  