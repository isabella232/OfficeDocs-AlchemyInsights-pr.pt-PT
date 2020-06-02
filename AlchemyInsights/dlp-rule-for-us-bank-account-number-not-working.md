---
title: Regra DLP para número de conta bancária dos EUA que não funciona
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
ms.openlocfilehash: b032a7c80e8b387114aeda95c4f6af7e57225517
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507345"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>DLP emite com números de contas bancárias dos EUA

**Importante**: durante estes tempos sem precedentes, estamos a tomar medidas para garantir que os serviços SharePoint Online e OneDrive permaneçam com elevada disponibilidade. Para obter mais informações, visite [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) (Ajustes Temporários de Funcionalidades do SharePoint Online).

**DLP emite com números de contas bancárias dos EUA**

Está a ter problemas com **a Prevenção de Perdas de Dados (DLP)** que não está a funcionar para conteúdos que contenham um **Número de Conta Bancária dos EUA** quando utilizar um tipo de informação sensível DLP em O365? Em caso afirmativo, certifique-se de que o seu conteúdo contém as informações necessárias para o que a política de DLP procura quando é avaliada.
  
Por exemplo, para uma política **de número de conta bancária dos EUA** configurada com um nível de confiança de 85%, são avaliadas as seguintes e devem ser detetadas para que a regra desencadeie:
  
- **[Formato:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 dígitos

- **[Padrão:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 dígitos consecutivos.

- **[Checkum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Não, não há Cheques.

- **[Definição:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** Uma política de DLP está 75% confiante de que é detetado este tipo de informação sensível se, dentro de uma proximidade de 300 caracteres:

  - A expressão regular Regex_usa_bank_account_number encontra conteúdo que corresponde ao padrão

  - Uma palavra-chave de Keyword_usa_Bank_Account é encontrada.

    Por exemplo, a seguinte amostra desencadearia a política de **número de conta bancária dos EUA:** Conta 78344011

Para obter mais informações sobre o que é necessário para que um **Número de Conta Bancária dos EUA** seja detetado para o seu conteúdo, consulte a seguinte secção neste artigo: O que os Tipos de [Informação Sensível procuram para o Número de Conta Bancária dos EUA](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)
  
Utilizando um tipo de informação sensível incorporado diferente, consulte o seguinte artigo para obter informações sobre o que é necessário para outros tipos: [O que os Tipos de Informação Sensível procuram](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  