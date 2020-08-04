---
title: Resolução de problemas de autenticação do cliente implantação de certificados de autenticação de clientes
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: 698329d7705af320c9f679b92532b58ac84e6624
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555302"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>Resolução de problemas de autenticação do cliente implantação de certificados de autenticação de clientes

Os perfis de certificados de cliente Intune NDES/SCEP e PKCS/PFX são comumente utilizados em conjunto com outros tipos de perfis, tais como Wifi, VPN e e-mail para permitir que os utilizadores autentem a autenticação aos recursos corporativos. Quando esses tipos de perfis estão ligados a um perfil de certificado de cliente dependem da implementação bem sucedida desse perfil.

A configuração inicial da infraestrutura e a configuração associada do perfil do Certificado de Cliente requerem frequentemente uma resolução de problemas. Para um guia passo a passo para a configuração bem sucedida do conector NDES e orientação de resolução de problemas para isolar problemas com a implantação de certificados, consulte: 

- [Configure a infraestrutura para apoiar o SCEP com a Intune](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [Visão geral para resolução de perfis de certificado SCEP com o Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

Utilize os scripts de powershell referenciados para ajudar a verificar a sua configuração. Para obter mais informações, consulte os scripts de [verificação do conector do Certificado Intune](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).

  
**Outras questões comuns**

**Quando tento instalar o conector de certificado Intune no servidor de conector NDES, recebo a mensagem: "A palavra-passe no pedido de certificado não pode ser verificada. Pode já ter sido usado. Obtenha uma nova senha para submeter com este pedido."**  

Esta mensagem significa que é necessário executar a instalação do conector do certificado como Administrador.

Em alguns ambientes, os servidores onde o Certificado Intune funciona devem utilizar um servidor proxy para se ligar ao Intune, pelo que o Conector de Certificado deve utilizar um representante. Em algumas circunstâncias, o Conector NDES ignora as configurações configuradas por procuração, e pode ser necessário configurar as definições de procuração enquanto funciona no contexto de segurança do Sistema Local. 
 
A solução é executar o Internet Explorer como SYSTEM e configurar um proxy no IE. Após um reinício do Serviço de Conector Intune, o Conector NDES liga-se ao Intune.

**Os dispositivos de utilizador deixaram de receber certificados SCEP da NDES.**

É possível que o certificado de autenticação do Cliente emitido para o servidor NDES, e especificado durante a instalação do conector NDES, tenha expirado ou esteja em falta. Para resolver: 
 
1. Desinstale o conector NDES.  
2. Utilize estes dados para solicitar um novo certificado de autenticação do cliente ou autenticação do servidor: 
 
    - Nome do assunto: CN=fqdn externo  
    - Nome alternativo do assunto (ambos são necessários): DNS=fqdn externo, DNS=fqdn interno 
 
3. Volte a instalar o conector NDES com o novo certificado.