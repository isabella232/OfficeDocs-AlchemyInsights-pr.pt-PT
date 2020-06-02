---
title: Regra do DLP para a SSN não funcionar
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 35859bce89ef1ae9b6a9e706fc316b0ee6cd27d1
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507381"
---
# <a name="dlp-issues-with-social-security-numbers"></a>Problemas de DLP com números de Segurança Social

**Importante**: durante estes tempos sem precedentes, estamos a tomar medidas para garantir que os serviços SharePoint Online e OneDrive permaneçam com elevada disponibilidade. Para obter mais informações, visite [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) (Ajustes Temporários de Funcionalidades do SharePoint Online).

**Problemas de DLP com SSNs**

Está a ter problemas com **a Prevenção de Perdas de Dados (DLP)** que não está a trabalhar para conteúdos que contenham um **Número de Segurança Social (SSN)** quando utiliza um tipo de informação sensível na Microsoft 365? Em caso afirmativo, certifique-se de que o seu conteúdo contém as informações necessárias para o que a política do DLP está a procurar. 
  
Por exemplo, para uma política da SSN configurada com um nível de confiança de 85%, são avaliadas as seguintes e devem ser detetadas para que a regra desencadeie:
  
- **[Formato:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 dígitos, que podem estar num padrão formatado ou não equipado

- **[Padrão:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Quatro funções procuram SSNs em quatro padrões diferentes:

  - Func_ssn encontra SSNs com formatação forte pré-2011 que são formatadas com traços ou espaços (ddd-ddd-dddd OU ddd ddd dddd)

  - Func_unformatted_ssn encontra SSNs com formatação forte pré-2011 que não são formatadas como nove dígitos consecutivos (dddddddd)

  - Func_randomized_formatted_ssn encontra SSNs pós-2011 que são formatadas com traços ou espaços (ddd-ddd-dddd OR ddd ddd dddd)

  - Func_randomized_unformatted_ssn encontra SSNs pós-2011 que não são formatadas como nove dígitos consecutivos (ddddddd)

- **[Checkum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Não, não há Cheques.

- **[Definição:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** Uma política de DLP está 85% confiante de que é detetado este tipo de informação sensível se, dentro de uma proximidade de 300 caracteres:

  - A [função Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) encontra conteúdo que corresponda ao padrão.

  - Uma palavra-chave de [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) é encontrada. Exemplos de palavras-chave incluem: *Segurança Social, Segurança Social#, Soc Sec ,SSN* . Por exemplo, a seguinte amostra desencadearia para a política DLP SSN: **SSN: 489-36-8350**
  
Para obter mais informações sobre o que é necessário para que as SSNs sejam detetadas para o seu conteúdo, consulte a seguinte secção neste artigo: [O que os Tipos de Informação Sensível procuram por SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
Utilizando um tipo de informação sensível incorporado diferente, consulte o seguinte artigo para obter informações sobre o que é necessário para outros tipos: [O que os Tipos de Informação Sensível procuram](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  