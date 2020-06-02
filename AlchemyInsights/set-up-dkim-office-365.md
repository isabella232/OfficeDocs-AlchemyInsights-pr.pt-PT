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
ms.openlocfilehash: 0acaed476dbd06bc933bf466f9bf6116413a44bb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509395"
---
# <a name="setup-dkim"></a>Configuração DKIM

As instruções completas para configurar o DKIM para domínios personalizados no Microsoft 365 estão [aqui](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

1. Para **cada** domínio personalizado, é necessário criar **dois** registos DKIM CNAME no serviço de hospedagem DNS do seu domínio (normalmente, o registo de domínio). Por exemplo, contoso.com e fourthcoffee.com requerem quatro registos DKIM CNAME: dois para contoso.com e dois para fourthcoffee.com.

   Os registos DKIM CNAME para **cada** domínio personalizado utilizam os seguintes formatos:

   - **Nome do anfitrião:**`selector1._domainkey.<CustomDomain>`

     **Pontos para endereço ou valor:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Nome do anfitrião:**`selector2._domainkey.<CustomDomain>`

     **Pontos para endereço ou valor:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\>é o texto à esquerda do `.mail.protection.outlook.com` registo MX personalizado para o domínio personalizado (por exemplo, `contoso-com` para o domínio contoso.com). \<InitialDomain\>é o domínio que usou quando se inscreveu no Microsoft 365 (por exemplo, contoso.onmicrosoft.com).

2. Depois de ter criado os registos CNAME para os seus domínios personalizados, complete as seguintes instruções:

   a. [iniciar sôm no Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) com o seu trabalho ou conta escolar.

   b. Selecione o ícone do iniciador de aplicações no canto superior esquerdo e selecione **Administrador**.

   c. Na navegação de baixo-esquerda, expanda **o Administrador** e escolha **o Exchange.**

   d. Vá para a **Proteção**  >  **DKIM**.

   e. Selecione o domínio e, em seguida, escolha **Ativar** **para iniciar mensagens para este domínio com assinaturas DKIM**. Repita este passo para cada domínio personalizado.
