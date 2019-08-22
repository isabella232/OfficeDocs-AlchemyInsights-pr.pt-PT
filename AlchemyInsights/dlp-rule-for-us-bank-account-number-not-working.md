---
title: Regra do DLP para nós número da conta bancária não funcionar
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 0a32708b5ac8d95ec6777ada2d151a15f90d65bf
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529889"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>Problemas do DLP com números de conta bancária-nos

Está a ter problemas com o **Data Loss Prevention (DLP)** não funcionar para o conteúdo que contenha um **Número de conta bancária nos e.u.a.** , quando utilizar um tipo de informações sensíveis do DLP em O365? Nesse caso, certifique-se o conteúdo contém as informações necessárias para que a política do DLP está à procura quando é avaliado.
  
Por exemplo, para uma política de **Número de conta bancária nos e.u.a.** configurada com um nível de confiança de 85%, a seguir é avaliados e deve ser detectada para a regra accionar:
  
- **[Formato:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 dígitos

- **[Padrão:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 dígitos consecutivos.

- **[Soma de verificação:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Não, não existe nenhum soma de verificação

- **[Definição:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** Uma política do DLP corresponde a 75% de certeza de que detectou este tipo de informações sensíveis se, num raio de 300 caracteres:

  - A expressão normal Regex_usa_bank_account_number localiza conteúdo que corresponda ao padrão

  - Foi encontrada uma palavra-chave de Keyword_usa_Bank_Account.

    Por exemplo, o seguinte exemplo daria origem para a política de **Número de conta bancária nos e.u.a.** : 78344011 de conta corrente

Para mais informações sobre o que é necessário para um **Número de conta bancária nos e.u.a.** ser detectado para o seu conteúdo, consulte a secção seguinte deste artigo: [O que o sensíveis a maiúsculas e tipos de informação procure o número de conta bancária nos e.u.a.](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)
  
Utilizando um tipo de informações sensíveis incorporados diferentes, consulte o artigo seguinte para obter informações sobre o que é necessário para outros tipos: [Procurar o que o sensíveis a maiúsculas e tipos de informação](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  