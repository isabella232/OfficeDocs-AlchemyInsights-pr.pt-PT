---
title: Regra do DLP para número de conta bancária dos EUA não funciona
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 45aa50f6c3505468e902e58faf698205f93f9264
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704050"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>DLP emite com números de conta bancária dos EUA

**Importante**: durante estes tempos sem precedentes, estamos a tomar medidas para garantir que os serviços SharePoint Online e OneDrive permaneçam com elevada disponibilidade. Para obter mais informações, visite [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) (Ajustes Temporários de Funcionalidades do SharePoint Online).

**DLP emite com números de conta bancária dos EUA**

Está a ter problemas com a Prevenção de Perdas de **Dados (DLP)** que não está a trabalhar para conteúdos que contenham um **Número de Conta Bancária dos EUA** ao utilizar um tipo de informação sensível dLP em O365? Em caso afirmativo, certifique-se de que o seu conteúdo contém as informações necessárias para o que a política do DLP procura quando é avaliada.
  
Por exemplo, para uma política de número de **conta bancária dos EUA** configurada com um nível de confiança de 85%, são avaliados e devem ser detetados para que a regra desencadeie:
  
- **[Formato:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 dígitos

- **[Padrão:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 dígitos consecutivos.

- **[Chequeum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Não, não há Checksum.

- **[Definição:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** Uma política de DLP está 75% confiante de que detetou este tipo de informação sensível se, dentro de uma proximidade de 300 caracteres:

  - A expressão regular Regex_usa_bank_account_number encontra conteúdo que corresponda ao padrão

  - Uma palavra-chave de Keyword_usa_Bank_Account é encontrada.

    Por exemplo, a seguinte amostra seria desencadeada para a política do número de **conta bancária dos EUA:** Conta de verificação 78344011

Para obter mais informações sobre o que é necessário para que um Número de **Conta Bancária dos EUA** seja detetado para o seu conteúdo, consulte a seguinte secção neste artigo: O que os Tipos de [Informação Sensível procuram para](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number) o Número de Conta Bancária dos EUA
  
Utilizando um tipo de informação sensível incorporado diferente, consulte o seguinte artigo para obter informações sobre o que é necessário para outros tipos: O que os Tipos de [Informação Sensível procuram](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  