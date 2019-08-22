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
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="7026c-102">Problemas do DLP com números de conta bancária-nos</span><span class="sxs-lookup"><span data-stu-id="7026c-102">DLP issues with US Bank Account Numbers</span></span>

<span data-ttu-id="7026c-103">Está a ter problemas com o **Data Loss Prevention (DLP)** não funcionar para o conteúdo que contenha um **Número de conta bancária nos e.u.a.** , quando utilizar um tipo de informações sensíveis do DLP em O365?</span><span class="sxs-lookup"><span data-stu-id="7026c-103">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="7026c-104">Nesse caso, certifique-se o conteúdo contém as informações necessárias para que a política do DLP está à procura quando é avaliado.</span><span class="sxs-lookup"><span data-stu-id="7026c-104">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="7026c-105">Por exemplo, para uma política de **Número de conta bancária nos e.u.a.** configurada com um nível de confiança de 85%, a seguir é avaliados e deve ser detectada para a regra accionar:</span><span class="sxs-lookup"><span data-stu-id="7026c-105">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="7026c-106">**[Formato:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 dígitos</span><span class="sxs-lookup"><span data-stu-id="7026c-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="7026c-107">**[Padrão:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 dígitos consecutivos.</span><span class="sxs-lookup"><span data-stu-id="7026c-107">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="7026c-108">**[Soma de verificação:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Não, não existe nenhum soma de verificação</span><span class="sxs-lookup"><span data-stu-id="7026c-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="7026c-109">**[Definição:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** Uma política do DLP corresponde a 75% de certeza de que detectou este tipo de informações sensíveis se, num raio de 300 caracteres:</span><span class="sxs-lookup"><span data-stu-id="7026c-109">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="7026c-110">A expressão normal Regex_usa_bank_account_number localiza conteúdo que corresponda ao padrão</span><span class="sxs-lookup"><span data-stu-id="7026c-110">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="7026c-111">Foi encontrada uma palavra-chave de Keyword_usa_Bank_Account.</span><span class="sxs-lookup"><span data-stu-id="7026c-111">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="7026c-112">Por exemplo, o seguinte exemplo daria origem para a política de **Número de conta bancária nos e.u.a.** : 78344011 de conta corrente</span><span class="sxs-lookup"><span data-stu-id="7026c-112">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="7026c-113">Para mais informações sobre o que é necessário para um **Número de conta bancária nos e.u.a.** ser detectado para o seu conteúdo, consulte a secção seguinte deste artigo: [O que o sensíveis a maiúsculas e tipos de informação procure o número de conta bancária nos e.u.a.](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="7026c-113">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span></span>
  
<span data-ttu-id="7026c-114">Utilizando um tipo de informações sensíveis incorporados diferentes, consulte o artigo seguinte para obter informações sobre o que é necessário para outros tipos: [Procurar o que o sensíveis a maiúsculas e tipos de informação](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="7026c-114">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  