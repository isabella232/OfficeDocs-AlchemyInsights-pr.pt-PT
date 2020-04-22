---
title: Configuração DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: d23a816d4eef065f800eaee60829d57dc1e7177f
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/21/2020
ms.locfileid: "43645683"
---
# <a name="setup-dkim"></a>Configuração DKIM

As instruções completas para configurar o DKIM para domínios personalizados no Microsoft 365 estão [aqui](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

1. Para **cada** domínio personalizado, é necessário criar **dois** registos DKIM CNAME no serviço de hospedagem DNS do seu domínio (tipicamente, o registo de domínio). Por exemplo, contoso.com e fourthcoffee.com requerem quatro registos DKIM CNAME: dois para contoso.com e dois para fourthcoffee.com.

   Os registos DKIM CNAME para **cada** domínio personalizado utilizam os seguintes formatos:

   - **Nome do anfitrião:**`selector1._domainkey.<CustomDomain>`

     **Pontos a endereçar ou valorizar:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Nome do anfitrião:**`selector2._domainkey.<CustomDomain>`

     **Pontos a endereçar ou valorizar:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> é o texto `.mail.protection.outlook.com` à esquerda no registo MX personalizado para `contoso-com` o domínio personalizado (por exemplo, para o domínio contoso.com). \<InitialDomain\> é o domínio que usou quando se inscreveu no Microsoft 365 (por exemplo, contoso.onmicrosoft.com).

2. Depois de ter criado os registos CNAME para os seus domínios personalizados, complete as seguintes instruções:

   a. [Inscreva-se na Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) com o seu trabalho ou conta escolar.

   b. Selecione o ícone do iniciador de aplicações no canto superior esquerdo e selecione **Administrador**.

   c. Na navegação de esquerda inferior, expanda o **Administrador** e escolha **o Exchange**.

   d. Vá para **a Proteção** > **DKIM.**

   e. Selecione o domínio e, em seguida, escolha **'Ativar** para **assinar mensagens' para este domínio com assinaturas DKIM**. Repita este passo para cada domínio personalizado.
