---
title: Resolução de problemas de autenticação do cliente implantação de certificados de autenticação de clientes
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: cecbd091447e63f2d5012ceaf96e050c92a171e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658997"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a><span data-ttu-id="f649b-102">Resolução de problemas de autenticação do cliente implantação de certificados de autenticação de clientes</span><span class="sxs-lookup"><span data-stu-id="f649b-102">Troubleshooting Client Authentication certificate deployment</span></span>

<span data-ttu-id="f649b-103">Os perfis de certificados de cliente Intune NDES/SCEP e PKCS/PFX são comumente utilizados em conjunto com outros tipos de perfis, tais como Wifi, VPN e e-mail para permitir que os utilizadores autentem a autenticação aos recursos corporativos.</span><span class="sxs-lookup"><span data-stu-id="f649b-103">Intune NDES/SCEP and PKCS/PFX Client certificates profiles are commonly used in conjunction with other profiles types such as Wifi, VPN, and email to allow users to authenticate to corporate resources.</span></span> <span data-ttu-id="f649b-104">Quando esses tipos de perfis estão ligados a um perfil de certificado de cliente dependem da implementação bem sucedida desse perfil.</span><span class="sxs-lookup"><span data-stu-id="f649b-104">When those profile types are linked to a client certificate profile are dependant on the successful deployment of that profile.</span></span>

<span data-ttu-id="f649b-105">A configuração inicial da infraestrutura e a configuração associada do perfil do Certificado de Cliente requerem frequentemente uma resolução de problemas.</span><span class="sxs-lookup"><span data-stu-id="f649b-105">Initial infrastructure setup and associated configuration of the Client Certificate profile often require troubleshooting.</span></span> <span data-ttu-id="f649b-106">Para um guia passo a passo para a configuração bem sucedida do conector NDES e orientação de resolução de problemas para isolar problemas com a implantação de certificados, consulte:</span><span class="sxs-lookup"><span data-stu-id="f649b-106">For a step-by-step guide to successful setup of the NDES connector and troubleshooting guidance to isolate issues with certificate deployment, see:</span></span> 

- [<span data-ttu-id="f649b-107">Configure a infraestrutura para apoiar o SCEP com a Intune</span><span class="sxs-lookup"><span data-stu-id="f649b-107">Configure infrastructure to support SCEP with Intune</span></span>](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [<span data-ttu-id="f649b-108">Visão geral para resolução de perfis de certificado SCEP com o Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="f649b-108">Overview for troubleshooting SCEP certificate profiles with Microsoft Intune</span></span>](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

<span data-ttu-id="f649b-109">Utilize os scripts de powershell referenciados para ajudar a verificar a sua configuração.</span><span class="sxs-lookup"><span data-stu-id="f649b-109">Use the referenced powershell scripts to help verify your configuration.</span></span> <span data-ttu-id="f649b-110">Para obter mais informações, consulte os scripts de [verificação do conector do Certificado Intune](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span><span class="sxs-lookup"><span data-stu-id="f649b-110">For more info, see [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span></span>

  
<span data-ttu-id="f649b-111">**Outras questões comuns**</span><span class="sxs-lookup"><span data-stu-id="f649b-111">**Other common issues**</span></span>

<span data-ttu-id="f649b-112">**Quando tento instalar o conector de certificado Intune no servidor de conector NDES, recebo a mensagem: "A palavra-passe no pedido de certificado não pode ser verificada. Pode já ter sido usado. Obtenha uma nova senha para submeter com este pedido."**</span><span class="sxs-lookup"><span data-stu-id="f649b-112">**When I try to install the Intune certificate connector on the NDES connector server, I get the message, "The password in the certificate request cannot be verified. It may have been used already. Obtain a new password to submit with this request."**</span></span>  

<span data-ttu-id="f649b-113">Esta mensagem significa que é necessário executar a instalação do conector do certificado como Administrador.</span><span class="sxs-lookup"><span data-stu-id="f649b-113">This message means that you need to run the certificate connector installation as an Administrator.</span></span>

<span data-ttu-id="f649b-114">Em alguns ambientes, os servidores onde o Certificado Intune funciona devem utilizar um servidor proxy para se ligar ao Intune, pelo que o Conector de Certificado deve utilizar um representante.</span><span class="sxs-lookup"><span data-stu-id="f649b-114">In some environments, the servers where the Intune Certificate runs must use a proxy server to connect to Intune, and so the Certificate Connector must use a proxy.</span></span> <span data-ttu-id="f649b-115">Em algumas circunstâncias, o Conector NDES ignora as configurações configuradas por procuração, e pode ser necessário configurar as definições de procuração enquanto funciona no contexto de segurança do Sistema Local.</span><span class="sxs-lookup"><span data-stu-id="f649b-115">In some circumstances, the NDES Connector ignores the configured proxy settings, and it might be necessary to configure the proxy settings while running in the security context of LocalSystem.</span></span> 
 
<span data-ttu-id="f649b-116">A solução é executar o Internet Explorer como SYSTEM e configurar um proxy no IE.</span><span class="sxs-lookup"><span data-stu-id="f649b-116">The solution is to run Internet Explorer as SYSTEM and configure a proxy in IE.</span></span> <span data-ttu-id="f649b-117">Após um reinício do Serviço de Conector Intune, o Conector NDES liga-se ao Intune.</span><span class="sxs-lookup"><span data-stu-id="f649b-117">After a restart of the Intune Connector Service, the NDES Connector connects to Intune.</span></span>

<span data-ttu-id="f649b-118">**Os dispositivos de utilizador deixaram de receber certificados SCEP da NDES.**</span><span class="sxs-lookup"><span data-stu-id="f649b-118">**User devices are no longer receiving SCEP certificates from NDES.**</span></span>

<span data-ttu-id="f649b-119">É possível que o certificado de autenticação do Cliente emitido para o servidor NDES, e especificado durante a instalação do conector NDES, tenha expirado ou esteja em falta.</span><span class="sxs-lookup"><span data-stu-id="f649b-119">It is possible that the Client Authentication certificate issued to the NDES server, and specified during the NDES connector installation, has expired or is missing.</span></span> <span data-ttu-id="f649b-120">Para resolver:</span><span class="sxs-lookup"><span data-stu-id="f649b-120">To resolve:</span></span> 
 
1. <span data-ttu-id="f649b-121">Desinstale o conector NDES.</span><span class="sxs-lookup"><span data-stu-id="f649b-121">Uninstall the NDES connector.</span></span>  
2. <span data-ttu-id="f649b-122">Utilize estes dados para solicitar um novo certificado de autenticação do cliente ou autenticação do servidor:</span><span class="sxs-lookup"><span data-stu-id="f649b-122">Use these details to request a new client authentication or server authentication certificate:</span></span> 
 
    - <span data-ttu-id="f649b-123">Nome do assunto: CN=fqdn externo</span><span class="sxs-lookup"><span data-stu-id="f649b-123">Subject name: CN=external fqdn</span></span>  
    - <span data-ttu-id="f649b-124">Nome alternativo do assunto (ambos são necessários): DNS=fqdn externo, DNS=fqdn interno</span><span class="sxs-lookup"><span data-stu-id="f649b-124">Subject alternative name (both are required): DNS=external fqdn, DNS=internal fqdn</span></span> 
 
3. <span data-ttu-id="f649b-125">Volte a instalar o conector NDES com o novo certificado.</span><span class="sxs-lookup"><span data-stu-id="f649b-125">Reinstall the NDES connector with the new certificate.</span></span>