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
# <a name="troubleshoot-saml-signing-certificate-issues"></a><span data-ttu-id="8c1b2-102">Problemas problemas saml assinatura de certificados</span><span class="sxs-lookup"><span data-stu-id="8c1b2-102">Troubleshoot SAML Signing certificate issues</span></span>

<span data-ttu-id="8c1b2-103">Para resolver a emissão do certificado de assinatura SAML, execute os seguintes passos recomendados:</span><span class="sxs-lookup"><span data-stu-id="8c1b2-103">To resolve SAML Signing certificate issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="8c1b2-104">Quando adicionar uma aplicação empresarial que suporta sSO, a Azure gerará um certificado chamado [certificado de assinatura SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications).</span><span class="sxs-lookup"><span data-stu-id="8c1b2-104">When you add an enterprise application which supports SSO, Azure will generate a certificate which is called the [SAML Signing certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications).</span></span> <span data-ttu-id="8c1b2-105">Este certificado tem uma data de validade de 3 anos.</span><span class="sxs-lookup"><span data-stu-id="8c1b2-105">This certificate has an expiration date of 3 years.</span></span> <span data-ttu-id="8c1b2-106">Para alterar a data de validade do seu certificado, consulte Personalizar a data de [validade do certificado da federação e entregá-la para um novo certificado](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).</span><span class="sxs-lookup"><span data-stu-id="8c1b2-106">To change the expiration date of your certificate, see [Customize the expiration date for your federation certificate and roll it over to a new certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).</span></span>
2. <span data-ttu-id="8c1b2-107">A Azure utilizará este certificado para assinar os tokens SAML solicitados pelo pedido e enviá-lo para o pedido de sSO bem sucedido.</span><span class="sxs-lookup"><span data-stu-id="8c1b2-107">Azure will use this certificate to sign the SAML tokens requested by the application and send it over to the application for a successful SSO.</span></span> <span data-ttu-id="8c1b2-108">Para que isto seja concluído, faça o download do certificado do portal Azure e envie-o ao fornecedor de aplicações para completar o processo SSO.</span><span class="sxs-lookup"><span data-stu-id="8c1b2-108">In order for this to complete, download the certificate from the Azure portal and send it to the application vendor to complete the SSO process.</span></span>

<span data-ttu-id="8c1b2-109">Após este processo concluído, o seu pedido confiará neste certificado e todos os tokens SAML assinados por este certificado serão aceites pelo pedido.</span><span class="sxs-lookup"><span data-stu-id="8c1b2-109">After this process completes your application will trust this certificate and all the SAML tokens signed by this certificate will be accepted by the application.</span></span>

3. <span data-ttu-id="8c1b2-110">Se este certificado expirar, crie um novo certificado, atualize-o ao fornecedor de aplicações e, em seguida, torne-o ativo no lado do Azure.</span><span class="sxs-lookup"><span data-stu-id="8c1b2-110">If this certificate expires, create a new certificate, update it to the application vendor and then make it active on the Azure side.</span></span> <span data-ttu-id="8c1b2-111">Para mais informações, consulte [Renovar um certificado que em breve expirará.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire)</span><span class="sxs-lookup"><span data-stu-id="8c1b2-111">For more information, see [Renew a certificate that will soon expire](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).</span></span>

> [!NOTE]
> <span data-ttu-id="8c1b2-112">Se o certificado expirar, o utilizador não será bloqueado.</span><span class="sxs-lookup"><span data-stu-id="8c1b2-112">If the certificate expires, the user will not be blocked.</span></span>

4. <span data-ttu-id="8c1b2-113">[Adicione um endereço de e-mail para notificações](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) a receber antes do certificado atual expirar.</span><span class="sxs-lookup"><span data-stu-id="8c1b2-113">[Add an email address for notifications](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) to be received before the current certificate expires.</span></span>

> [!NOTE]
> <span data-ttu-id="8c1b2-114">O passo 4 é opcional.</span><span class="sxs-lookup"><span data-stu-id="8c1b2-114">Step-4 is an optional one.</span></span>

5. <span data-ttu-id="8c1b2-115">Altere as opções de assinatura de certificado SAML de uma aplicação e o algoritmo de assinatura de certificado.</span><span class="sxs-lookup"><span data-stu-id="8c1b2-115">Change an application's SAML certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="8c1b2-116">Para obter mais informações, consulte [opções de assinatura de certificado de alteração e algoritmo de assinatura.](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)</span><span class="sxs-lookup"><span data-stu-id="8c1b2-116">For more information, see [Change certificate signing options and signing algorithm](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>

