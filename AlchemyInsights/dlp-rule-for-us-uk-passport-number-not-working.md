---
title: Regra do DLP para e.u.a. / número do passaporte Reino Unido não funcionar
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
ms.openlocfilehash: 0567e9521507bcc192b187d0e5a8a0658332ff99
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/28/2019
ms.locfileid: "35389552"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="a3d60-102">Problemas com DLP - e.u.a. / números de Passport do Reino Unido</span><span class="sxs-lookup"><span data-stu-id="a3d60-102">Problems with DLP - US/UK Passport Numbers</span></span>

<span data-ttu-id="a3d60-103">Está a ter problemas com o **Data Loss Prevention (DLP)** não funcionar para que contenha conteúdo uma **dos e.u.a. / número do passaporte UK** quando utilizar um tipo de informações sensíveis do DLP em O365?</span><span class="sxs-lookup"><span data-stu-id="a3d60-103">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK Passport Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="a3d60-104">Nesse caso, certifique-se o conteúdo contém as informações necessárias para que a política do DLP está à procura quando é avaliado.</span><span class="sxs-lookup"><span data-stu-id="a3d60-104">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="a3d60-105">Por exemplo, para um **dos e.u.a. / número do passaporte UK** política configurada com um nível de confiança de 75%, os seguintes são avaliados e deve ser detectados para a regra accionar</span><span class="sxs-lookup"><span data-stu-id="a3d60-105">For example, for a **US/UK Passport Number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="a3d60-106">**[Formato:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nove algarismos</span><span class="sxs-lookup"><span data-stu-id="a3d60-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span>

- <span data-ttu-id="a3d60-107">**[Padrão:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nove algarismos consecutivos.</span><span class="sxs-lookup"><span data-stu-id="a3d60-107">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="a3d60-108">**[Soma de verificação:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Não, não existe nenhum soma de verificação</span><span class="sxs-lookup"><span data-stu-id="a3d60-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="a3d60-109">**[Definição:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** Uma política do DLP corresponde a 75% de certeza de que detectou este tipo de informações sensíveis se, num raio de 300 caracteres:</span><span class="sxs-lookup"><span data-stu-id="a3d60-109">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="a3d60-110">A função Func_usa_uk_passport localiza conteúdo que corresponda ao padrão.</span><span class="sxs-lookup"><span data-stu-id="a3d60-110">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="a3d60-111">Foi encontrada uma palavra-chave de Keyword_passport.</span><span class="sxs-lookup"><span data-stu-id="a3d60-111">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="a3d60-112">Por exemplo, o seguinte exemplo daria origem para o **dos e.u.a. / número do passaporte UK** política: número de Estados Unidos Passport 123456789</span><span class="sxs-lookup"><span data-stu-id="a3d60-112">For example, the following sample would trigger for the **US/UK Passport Number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="a3d60-113">Para mais informações sobre o que é necessário para dos e.u.a. / número do passaporte UK para ser detectado para o seu conteúdo, consulte a secção seguinte deste artigo: [localizar o que o sensíveis a maiúsculas e tipos de informação dos e.u.a. / número do passaporte UK](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="a3d60-113">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="a3d60-114">Utilizando um tipo de informações sensíveis incorporados diferentes, consulte o artigo seguinte para obter informações sobre o que é necessário para outros tipos: [Procurar o que o sensíveis a maiúsculas e tipos de informação](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="a3d60-114">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  