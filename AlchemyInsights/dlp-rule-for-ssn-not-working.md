---
title: Regra DLP para SSN não funcionar
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
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 3f30998fb3bc4c5442e4e1541b87d88ecd7df6eef3a50e719fa5014eb86af39c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004993"
---
# <a name="dlp-issues-with-social-security-numbers"></a>Problemas de DLP com Números de Segurança Social

**Importante**: durante estes tempos sem precedentes, estamos a tomar medidas para garantir que os serviços SharePoint Online e OneDrive permaneçam com elevada disponibilidade. Para obter mais informações, visite [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) (Ajustes Temporários de Funcionalidades do SharePoint Online).

**Problemas de DLP com SSNs**

Está a ter problemas com a Prevenção de Perda de Dados **(DLP)** que não funciona em conteúdos que contenham um Número de Segurança **Social (SSN)** ao utilizar um tipo de informação confidencial no Microsoft 365? Se for o caso, certifique-se de que o seu conteúdo contém as informações necessárias para o aspas da política DLP. 
  
Por exemplo, para uma política SSN configurada com um nível de confiança de 85%, o seguinte é avaliado e tem de ser detetado para que a regra acione:
  
- **[Formato:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 dígitos, que podem estar num padrão formatado ou não formatado

- **[Padrão:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Quatro funções procuram SSNs em quatro padrões diferentes:

  - Func_ssn encontra SSNs com uma formatação forte pré-2011 formatada com traços ou espaços (ddd-ddd-dddd OU ddd ddd dddd)

  - Func_unformatted_ssn encontra SSNs com uma formatação forte pré-2011 não formatada como nove dígitos consecutivos (ddddddddd)

  - Func_randomized_formatted_ssn encontra SSNs do pós-2011 formatados com traços ou espaços (ddd-ddd-dddd OU ddd ddd dddd)

  - Func_randomized_unformatted_ssn encontrar SSNs pós-2011 que não foram formatados como nove dígitos consecutivos (ddddddddd)

- **[Somar Verificação:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Não, não existe Soão Desmarcação

- **[Definição:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** Uma política DLP tem 85% de confiança de que detetou este tipo de informações confidenciais se, dentro de uma proximidade de 300 carateres:

  - A [função Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) encontrar conteúdo que corresponda ao padrão.

  - Foi encontrada uma [palavra-Keyword_ssn malhe.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) Exemplos de palavras-chave incluem:  *Segurança Social, Segurança Social#, Soc Seg , SSN*  . Por exemplo, a seguinte amostra aciona a política **SSN DLP: SSN: 489-36-8350**
  
Para obter mais informações sobre o que é necessário para que os SSNs sejam detetados para o seu conteúdo, consulte a seguinte secção neste artigo: O que os Tipos de Informação Confidenciais procuram [por SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
Utilizando um tipo de informações confidenciais incorporado diferente, consulte o seguinte artigo para obter informações sobre o que é necessário para outros tipos: O que procuram os Tipos de Informação [Confidenciais](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  