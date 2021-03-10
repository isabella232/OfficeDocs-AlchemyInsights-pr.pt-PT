---
title: Problemas de resolução de problemas SAML que assinam problemas com os certificados
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9406"
- "9004341"
ms.openlocfilehash: 3bc8b2e751395b8a099fb5079ad40c5c93222e0e
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694446"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a>Problemas problemas saml assinatura de certificados

Para resolver a emissão do certificado de assinatura SAML, execute os seguintes passos recomendados:

1. Quando adicionar uma aplicação empresarial que suporta sSO, a Azure gerará um certificado chamado [certificado de assinatura SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications). Este certificado tem uma data de validade de 3 anos. Para alterar a data de validade do seu certificado, consulte Personalizar a data de [validade do certificado da federação e entregá-la para um novo certificado](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).
2. A Azure utilizará este certificado para assinar os tokens SAML solicitados pelo pedido e enviá-lo para o pedido de sSO bem sucedido. Para que isto seja concluído, faça o download do certificado do portal Azure e envie-o ao fornecedor de aplicações para completar o processo SSO.

Após este processo concluído, o seu pedido confiará neste certificado e todos os tokens SAML assinados por este certificado serão aceites pelo pedido.

3. Se este certificado expirar, crie um novo certificado, atualize-o ao fornecedor de aplicações e, em seguida, torne-o ativo no lado do Azure. Para mais informações, consulte [Renovar um certificado que em breve expirará.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire)

> [!NOTE]
> Se o certificado expirar, o utilizador não será bloqueado.

4. [Adicione um endereço de e-mail para notificações](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) a receber antes do certificado atual expirar.

> [!NOTE]
> O passo 4 é opcional.

5. Altere as opções de assinatura de certificado SAML de uma aplicação e o algoritmo de assinatura de certificado. Para obter mais informações, consulte [opções de assinatura de certificado de alteração e algoritmo de assinatura.](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)

