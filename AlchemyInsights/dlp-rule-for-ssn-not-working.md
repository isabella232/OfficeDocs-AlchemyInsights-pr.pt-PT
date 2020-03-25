---
title: Regra do DLP para a SSN não funcionar
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 0b83a858975ffe1bb70f16a7452a13d57dff5340
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932546"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP emite com números de Segurança Social

**Importante**: Muitos clientes SharePoint Online e OneDrive executam aplicações críticas ao negócio contra o serviço que executa em segundo plano. Estes incluem migração de conteúdos, Prevenção de Perdas de Dados (DLP) e soluções de backup. Durante estes tempos sem precedentes, estamos a tomar medidas para garantir que os serviços SharePoint Online e OneDrive permanecem altamente disponíveis e fiáveis para os seus utilizadores que dependem mais do serviço do que nunca em cenários de trabalho remoto.

Em apoio a este objetivo, implementámos limites de estrangulamento mais apertados em aplicações de fundo (soluções de migração, DLP e backup) durante o dia da semana. Deve esperar que estas aplicações atinjam uma entrada muito limitada durante estes tempos. No entanto, durante as horas de noite e fim de semana para a região, o serviço estará pronto para processar um volume significativamente maior de pedidos de aplicações de fundo.

**DLP problemas com SSNs**

Está a ter problemas com a Prevenção de Perdas de **Dados (DLP)** que não está a trabalhar para conteúdos que contenham um Número de **Segurança Social (SSN)** quando utilizar um tipo de informação sensível no Office 365? Em caso afirmativo, certifique-se de que o seu conteúdo contém as informações necessárias para o que a política do DLP está a procurar. 
  
Por exemplo, para uma política SSN configurada com um nível de confiança de 85%, são avaliados e devem ser detetados para que a regra desencadeie:
  
- **[Formato:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 dígitos, que podem estar num padrão formatado ou não formatado

- **[Padrão:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Quatro funções procuram SSNs em quatro padrões diferentes:

  - Func_ssn encontra SSNs com formatação forte pré-2011 que são formatadas com traços ou espaços (ddd-ddddd ddddd ddddd)

  - Func_unformatted_ssn encontra SSNs com formatação forte pré-2011 que não são formatadas como nove dígitos consecutivos (dddddddddd)

  - Func_randomized_formatted_ssn encontra SSNs pós-2011 que são formatados com traços ou espaços (ddd-ddddd or dddddd dddddd)

  - Func_randomized_unformatted_ssn encontra SSNs pós-2011 que não são formatadas como nove dígitos consecutivos (ddddddddddd)

- **[Chequeum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Não, não há Checksum.

- **[Definição:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** Uma política de DLP está 85% confiante de que detetou este tipo de informação sensível se, dentro de uma proximidade de 300 caracteres:

  - A [função Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) encontra conteúdo que corresponda ao padrão.

  - Uma palavra-chave de [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) é encontrada. Exemplos de palavras-chave incluem: *Segurança Social, Segurança Social#, Soc Sec ,SSN* . Por exemplo, a seguinte amostra seria desencadeada para a política DLP SSN: **SSN: 489-36-8350**
  
Para obter mais informações sobre o que é necessário para que as SSNs sejam detetadas para o seu conteúdo, consulte a seguinte secção neste artigo: O que os Tipos de [Informação Sensível procuram por SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)
  
Utilizando um tipo de informação sensível incorporado diferente, consulte o seguinte artigo para obter informações sobre o que é necessário para outros tipos: O que os Tipos de [Informação Sensível procuram](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  