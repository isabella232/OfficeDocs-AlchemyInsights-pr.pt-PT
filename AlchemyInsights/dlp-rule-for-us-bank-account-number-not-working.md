---
title: Regra do DLP para nós número da conta bancária não funcionar
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 9ebfa6bc09cef9ab7c30bddb4fcb8b6be3ab55a5
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/12/2019
ms.locfileid: "29916427"
---
<span data-ttu-id="39602-p101">Está a ter problemas com o **Data Loss Prevention (DLP)** não funcionar para o conteúdo que contenha um **Número de conta bancária nos e.u.a.** , quando utilizar um tipo de informações sensíveis do DLP em O365? Nesse caso, certifique-se o conteúdo contém as informações necessárias para que a política do DLP está à procura quando é avaliado.</span><span class="sxs-lookup"><span data-stu-id="39602-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365? If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span> 
  
<span data-ttu-id="39602-104">Por exemplo, para uma política de **Número de conta bancária nos e.u.a.** configurada com um nível de confiança de 85%, a seguir é avaliados e deve ser detectada para a regra accionar:</span><span class="sxs-lookup"><span data-stu-id="39602-104">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span> 
  
- <span data-ttu-id="39602-105">**[Formato:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 dígitos</span><span class="sxs-lookup"><span data-stu-id="39602-105">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 digits</span></span> 
    
- <span data-ttu-id="39602-106">**[Padrão:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 dígitos consecutivos.</span><span class="sxs-lookup"><span data-stu-id="39602-106">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 consecutive digits.</span></span> 
    
- <span data-ttu-id="39602-107">**[Soma de verificação:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Não, não existe nenhum soma de verificação</span><span class="sxs-lookup"><span data-stu-id="39602-107">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span> 
    
- <span data-ttu-id="39602-108">**[Definição:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** Uma política do DLP corresponde a 75% de certeza de que detectou este tipo de informações sensíveis se, num raio de 300 caracteres:</span><span class="sxs-lookup"><span data-stu-id="39602-108">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="39602-109">A expressão normal Regex_usa_bank_account_number localiza conteúdo que corresponda ao padrão</span><span class="sxs-lookup"><span data-stu-id="39602-109">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>
    
  - <span data-ttu-id="39602-110">Foi encontrada uma palavra-chave de Keyword_usa_Bank_Account.</span><span class="sxs-lookup"><span data-stu-id="39602-110">A keyword from Keyword_usa_Bank_Account is found.</span></span>
    
    <span data-ttu-id="39602-111">Por exemplo, o seguinte exemplo daria origem para a política de **Número de conta bancária nos e.u.a.** : 78344011 de conta corrente</span><span class="sxs-lookup"><span data-stu-id="39602-111">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span> 
    
<span data-ttu-id="39602-112">Para mais informações sobre o que é necessário para um **Número de conta bancária nos e.u.a.** ser detectado para o seu conteúdo, consulte a secção seguinte deste artigo: [O que o sensíveis a maiúsculas e tipos de informação procure o número de conta bancária nos e.u.a.](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="39602-112">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span></span>
  
<span data-ttu-id="39602-113">Utilizando um tipo de informações sensíveis incorporados diferentes, consulte o artigo seguinte para obter informações sobre o que é necessário para outros tipos: [Procurar o que o sensíveis a maiúsculas e tipos de informação](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="39602-113">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

