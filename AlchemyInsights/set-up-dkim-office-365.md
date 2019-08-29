---
title: O programa de configuração DKIM no Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: dd908db6a4bc1739b3c1cff059387034d67e093d
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666275"
---
# <a name="setup-dkim-in-office-365"></a>O programa de configuração DKIM no Office 365

As instruções completas para configurar DKIM são domínios personalizados no Office 365 [aqui](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

1. Para **cada** domínio personalizado, tem de criar **dois** registos DKIM CNAME no serviço de alojamento do domínio DNS (normalmente, o escrivão do domínio). Por exemplo, contoso.com e fourthcoffee.com requerem quatro registos DKIM CNAME: duas para contoso.com e dois para fourthcoffee.com.

   Os registos DKIM CNAME para **cada** domínio personalizado, utilize os seguintes formatos:

   - **Nome de anfitrião**:`selector1._domainkey.<CustomDomain>`

     **Pontos para o endereço ou de valor**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Nome de anfitrião**:`selector2._domainkey.<CustomDomain>`

     **Pontos para o endereço ou de valor**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> é o texto à esquerda da `.mail.protection.outlook.com` no registo MX personalizado para o domínio personalizado (por exemplo, `contoso-com` para o domínio contoso.com). \<InitialDomain\> é o domínio que utilizou quando se inscreve para Office 365 (por exemplo, contoso.onmicrosoft.com).

2. Depois de ter criado os registos CNAME para os domínios personalizados, conclua as seguintes instruções:

   a. [Inicie sessão no Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) com a sua conta escolar ou profissional.

   b. Selecione o ícone do iniciador de aplicações no canto superior esquerdo e selecione **Administrador**.

   c. No painel de navegação no canto inferior esquerdo, expanda **Administração** e escolha o **Exchange**.

   d. Vá para a **protecção** > **DKIM**.

   e. Seleccione o domínio e, em seguida, escolher **Activar** para **mensagens de início de sessão para este domínio com assinaturas DKIM**. Repita este passo para cada domínio personalizado.
