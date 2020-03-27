---
title: Regra dLP para número de passaporte dos EUA/Reino Unido não funciona
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 534e258c31a9a71c618765511487487c53f455b5
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977117"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problemas com dlp - números de passaporte dos EUA/Reino Unido

**Importante**: Durante estes tempos sem precedentes, estamos a tomar medidas para garantir que os serviços SharePoint Online e OneDrive permanecem altamente disponíveis – Visite os Ajustes de [FuncionalidadeS Temporárias Online SharePoint](https://aka.ms/ODSPAdjustments) para obter mais informações.

**DLP emite problemas com números de passaporte dos EUA/Reino Unido**

Está a ter problemas com a Prevenção de Perdas de **Dados (DLP)** que não está a trabalhar para conteúdos que contenham um número de **passaporte EUA/Reino Unido** ao utilizar um tipo de informação sensível dLP em O365? Em caso afirmativo, certifique-se de que o seu conteúdo contém as informações necessárias para o que a política do DLP procura quando é avaliada.
  
Por exemplo, para uma política de número de **passaporte dos EUA/Reino Unido** configurada com um nível de confiança de 75%, são avaliados e devem ser detetados para que a regra desencadeie
  
- **[Formato:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nove dígitos

- **[Padrão:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nove dígitos consecutivos

- **[Chequeum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Não, não há Checksum.

- **[Definição:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** Uma política de DLP está 75% confiante de que detetou este tipo de informação sensível se, dentro de uma proximidade de 300 caracteres:

  - A função Func_usa_uk_passport encontra conteúdo que corresponda ao padrão.

  - Uma palavra-chave de Keyword_passport é encontrada.

    Por exemplo, a seguinte amostra seria desencadeada para a política de número de **passaporte dos EUA/Reino Unido:** Passaporte dos EUA número 123456789

Para obter mais informações sobre o que é necessário para que um número de passaporte dos EUA/Reino Unido seja detetado para o seu conteúdo, consulte a seguinte secção neste artigo: [O que os Tipos de Informação Sensível procuram para o Número de Passaporte supor EUA/Reino Unido](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
Utilizando um tipo de informação sensível incorporado diferente, consulte o seguinte artigo para obter informações sobre o que é necessário para outros tipos: O que os Tipos de [Informação Sensível procuram](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  