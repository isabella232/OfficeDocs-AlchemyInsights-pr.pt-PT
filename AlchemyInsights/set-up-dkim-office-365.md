---
title: Configurar DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 5dc90965516cc4d360b9be56c7737c6d134123ea8ac263b092559dd1416faff4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54108567"
---
# <a name="setup-dkim"></a>Configurar DKIM

As instruções completas para configurar o DKIM para domínios personalizados no Microsoft 365 estão [aqui.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)

1. Para **cada** domínio personalizado, tem de criar dois registos **CNAME** DKIM no serviço de registo DNS do seu domínio (normalmente, a registo de domínios). Por exemplo, contoso.com e fourthcoffee.com requerem quatro registos CNAME DKIM: dois para contoso.com e dois para fourthcoffee.com.

   Os registos CNAME DKIM para **cada domínio** personalizado utilizam os seguintes formatos:

   - **Nome do anfitrião:**`selector1._domainkey.<CustomDomain>`

     **Aponta para o endereço ou valor:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL:** 3600

   - **Nome do anfitrião:**`selector2._domainkey.<CustomDomain>`

     **Aponta para o endereço ou valor:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL:** 3600

   \<DomainGUID\> é o texto à esquerda do registo MX personalizado do domínio personalizado `.mail.protection.outlook.com` (por exemplo, para a caixa `contoso-com` de contoso.com). \<InitialDomain\>é o domínio que usou quando se inscreveu para Microsoft 365 (por exemplo, contoso.onmicrosoft.com).

2. Após criar os registos CNAME para os seus domínios personalizados, conclua as seguintes instruções:

   a. [inscreva-se no Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) com a sua conta escolar ou pessoal.

   b. Selecione o ícone do iniciador de aplicações no canto superior esquerdo e selecione **Administrador**.

   c. Na navegação no canto inferior esquerdo, expanda **Admin e** selecionar **Exchange**.

   d. Vá para **Protection**  >  **DKIM.**

   e. Selecione o domínio e, em seguida,  **selecione Ativar para Assinar mensagens para este domínio com assinaturas DKIM.** Repita este passo para cada domínio personalizado.
