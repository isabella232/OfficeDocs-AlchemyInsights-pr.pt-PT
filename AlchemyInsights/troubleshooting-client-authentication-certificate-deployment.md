---
title: Remoção da implementação do certificado de Autenticação de Cliente
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
ms.openlocfilehash: 78520b416a72a3c93a3d2e7726948d59f83e681d4f09078c2a3cefac7bf1db3d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020815"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>Remoção da implementação do certificado de Autenticação de Cliente

Os perfis de certificados de Cliente Intune NDES/SCEP e PKCS/PFX Client são geralmente utilizados em conjunto com outros tipos de perfis, como Wifi, VPN e e-mail, para permitir que os utilizadores autentiquem os recursos da empresa. Quando esses tipos de perfil estão ligados a um perfil de certificado de cliente dependem da implementação bem-sucedida nesse perfil.

A configuração inicial da infraestrutura e a configuração associada do perfil do Certificado de Cliente exigem muitas vezes remoção de problemas. Para um guia passo a passo sobre a configuração com êxito do conector NDES e orientação para reação de problemas para isolar problemas com a implementação de certificados, consulte: 

- [Configurar infraestrutura para suportar SCEP com o Intune](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [Overview for troubleshooting SCEP certificate profiles with Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

Utilize os scripts do PowerShell referenciados para ajudar a verificar a sua configuração. Para mais informações, consulte [Scripts de verificação do conector](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority)de Certificado do Intune.

  
**Outros problemas comuns**

**Quando tento instalar o conector de certificado do Intune no servidor de conector NDES, é-me enviada a mensagem "Não é possível verificar a palavra-passe no pedido de certificado. Já pode ter sido utilizado. Obtenha uma nova palavra-passe para submeter com este pedido."**  

Esta mensagem significa que tem de executar a instalação do conector de certificado como administrador.

Em alguns ambientes, os servidores onde o Certificado do Intune é executado têm de utilizar um servidor proxy para ligar ao Intune, pelo que o Conector de Certificados tem de utilizar um proxy. Em algumas circunstâncias, o Conector NDES ignora as definições de proxy configuradas e poderá ser necessário configurar as definições de proxy durante a execução no contexto de segurança do LocalSystem. 
 
A solução é executar o Internet Explorer como SISTEMA e configurar um proxy no IE. Após reiniciar o Serviço do Conector do Intune, o NDES Connector liga-se ao Intune.

**Os dispositivos de utilizador já não recebem certificados SCEP de NDES.**

É possível que o certificado de Autenticação de Cliente emitido para o servidor NDES e especificado durante a instalação do conector NDES tenha expirado ou estiver em falta. Para resolver: 
 
1. Desinstale o conector NDES.  
2. Utilize estes detalhes para pedir um novo certificado de autenticação de cliente ou de autenticação do servidor: 
 
    - Nome do assunto: CN=fqdn externo  
    - Nome alternativo do assunto (ambos são obrigatórios): DNS=fqdn externo, DNS=fqdn interno 
 
3. Reinstale o conector NDES com o novo certificado.