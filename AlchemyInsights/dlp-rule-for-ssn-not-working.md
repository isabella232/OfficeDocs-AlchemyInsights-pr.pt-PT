---
title: Regra do DLP para SSN não funcionar
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
ms.openlocfilehash: 757136c39700f12f40f839b29277a59b0e436f03
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529876"
---
# <a name="dlp-issues-with-social-security-numbers"></a>Problemas do DLP com números da Segurança Social

Está a ter problemas com o **Data Loss Prevention (DLP)** não funcionar para o conteúdo que contém um **Número da Segurança Social (SSN)** quando utilizar um tipo de informações sensíveis no Office 365? Se assim for, certifique-se que o conteúdo contém as informações necessárias para que a política do DLP está à procura. 
  
Por exemplo, para uma política de SSN configurada com um nível de confiança de 85%, a seguir é avaliados e deve ser detectada para a regra accionar:
  
- **[Formato:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 dígitos, que poderão ser um padrão formatado ou não formatado

- **[Padrão:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Quatro funções procure SSNs na quatro padrões diferentes:

  - Func_ssn localiza SSNs com pré-2011 forte formatação que são formatados com travessões ou espaços (ddd-dd-dddd ou ddd dd dddd)

  - Func_unformatted_ssn localiza SSNs com pré-2011 forte formatação que está formatada como nove dígitos consecutivos (ddddddddd)

  - Func_randomized_formatted_ssn localiza SSNs post 2011 formatados com travessões ou espaços (ddd-dd-dddd ou ddd dd dddd)

  - Func_randomized_unformatted_ssn localiza post 2011 SSNs que estão formatados como nove dígitos consecutivos (ddddddddd)

- **[Soma de verificação:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Não, não existe nenhum soma de verificação

- **[Definição:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** Uma política DLP é de 85% de certeza de que detectou este tipo de informações sensíveis se, num raio de 300 caracteres:

  - A [função Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) localiza conteúdo que corresponda ao padrão.

  - Foi encontrada uma palavra-chave de [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) . Inclui exemplos de palavras-chave: *Segurança Social, de Segurança Social #, seg. Soc, SSN* . Por exemplo, o seguinte exemplo daria origem para a política do DLP SSN: **SSN: 489-36-8350**
  
Para mais informações sobre o que é necessário para SSNs ser detectado para o seu conteúdo, consulte a secção seguinte deste artigo: [O que o sensíveis a maiúsculas e tipos de informação procure SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)
  
Utilizando um tipo de informações sensíveis incorporados diferentes, consulte o artigo seguinte para obter informações sobre o que é necessário para outros tipos: [Procurar o que o sensíveis a maiúsculas e tipos de informação](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  