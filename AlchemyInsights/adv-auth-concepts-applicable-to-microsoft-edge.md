---
title: Conceitos avançados de autenticação aplicáveis ao Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
ms.openlocfilehash: 241d594fac6664dd1e85fd60e30a6344c432555e
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573527"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Conceitos avançados de autenticação aplicáveis ao Microsoft Edge

Seguem-se os conceitos avançados de autenticação aplicáveis ao Microsoft Edge:

**Autenticação Proativa**

Quando ativar a política [ProactiveAuthEnabled,](https://go.microsoft.com/fwlink/?linkid=2134621) o Microsoft Edge tentará autenticar proactivamente os utilizadores inscritos através dos serviços da Microsoft. Em intervalos regulares, utilizará um serviço online para verificar se há um manifesto atualizado que contenha a configuração que rege a Autenticação Proactiva.

Benefícios: A autenticação proativa permite a autenticação em serviços-chave, como a Página do Separador Do Office New. Além disso, se bing é usado como motor de pesquisa, a Autenticação Proativa melhora o desempenho da barra de endereços e ajuda a gerar resultados de pesquisa personalizados às necessidades do seu negócio.

**Windows Hello CredUI para autenticação NTLM**

Se um único sign-on (SSO) não estiver disponível quando um website tentar assinar no utilizador através do mecanismo NTLM ou Negotiate, esta funcionalidade permitirá ao utilizador partilhar as credenciais de OS com o website e satisfazer o desafio de autenticação utilizando o UI do Windows Hello Cred. Este fluxo de entrada de sing-on aparecerá apenas no Windows 10 e apenas para utilizadores que não obtenham SSO durante um NTLM ou um desafio Negotiate.

**Utilize senhas guardadas para iniciar sôm automaticamente**

Os utilizadores que guardam palavras-passe no Microsoft Edge podem permitir o acesso automático aos websites onde guardaram credenciais. Os utilizadores podem ligar ou desligar esta funcionalidade em edge://settings/passwords, podendo configugá-la nas políticas do [gestor de passwords.](https://go.microsoft.com/fwlink/?linkid=2134622)
