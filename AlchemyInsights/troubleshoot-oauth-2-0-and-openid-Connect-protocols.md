---
title: Resolução de problemas Protocolos OAuth 2.0 e OpenID Connect
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9776"
- "9004342"
ms.openlocfilehash: d2f14d4d16bea890b564cdb9bd9ac3875c28d115
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037702"
---
# <a name="troubleshoot-oauth-20-and-openid-connect-protocols"></a>Resolução de problemas Protocolos OAuth 2.0 e OpenID Connect

Para resolver os problemas OAuth 2.0 e OpenID Connect, execute os seguintes passos recomendados:

Consulte os seguintes artigos relacionados com a configuração e resolução de problemas dos protocolos OAuth 2.0 e OpenID Connect:

- [Plataforma de identidade da Microsoft e fluxo de código de autorização OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) - Este artigo descreve como programar diretamente contra o **fluxo de código (PKCE)** na sua aplicação, utilizando qualquer idioma.
- [Plataforma de identidade da Microsoft e fluxo de credenciais de cliente OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) - Este artigo descreve como programar diretamente contra as credenciais do **cliente fluem** na sua aplicação.
- [Plataforma de identidade da Microsoft e Credenciais de Senha do Proprietário de Recursos OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth-ropc) - Este artigo descreve como programar diretamente contra o **fluxo ROPC** na sua aplicação.
    - A plataforma de identidade da Microsoft apenas suporta ROPC para inquilinos AZure AD, e não para contas pessoais. Isto significa que você deve usar um ponto final específico do inquilino **(ou https://login.microsoftonline.com/{TenantId_or_Name})** o ponto final das **organizações.**
    - As contas pessoais que são convidadas para um inquilino da AD Azure não podem usar o ROPC.
    - As contas que não têm senhas não podem entrar através do ROPC. Para este cenário, recomendamos que utilize um fluxo diferente para a sua aplicação, em vez disso.
    - Se os utilizadores precisarem de utilizar a [autenticação de vários fatores (MFA)](https://docs.microsoft.com/azure/active-directory/authentication/concept-mfa-howitworks) para iniciar sessão na aplicação, serão bloqueados.
    - O ROPC não é suportado em cenários [de federação de identidade híbrida](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-fed) (por exemplo, Azure AD e ADFS usados para autenticar contas no local). Se os utilizadores forem redirecionados para um fornecedor de identidade no local, o Azure AD não é capaz de testar o nome de utilizador e a palavra-passe contra esse fornecedor de identidade. No entanto, [a autenticação pass-through](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-pta) é suportada com ROPC.
    - Uma exceção a um cenário de federação de identidade híbrida seria o seguinte: A política home Realm Discovery com **AllowCloudPasswordValidation** definida para **TRUE** permitirá que o fluxo ROPC funcione para utilizadores federados quando a palavra-passe no local estiver sincronizada na nuvem. Para obter mais informações, consulte [Ativar a autenticação direta ropc dos utilizadores federados para aplicações antigas](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#enable-direct-ropc-authentication-of-federated-users-for-legacy-applications) 
- [Plataforma de identidade da Microsoft e OAuth 2.0 Em nome-of-flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow) - Este artigo descreve como programar diretamente contra o **fluxo em nome da (OBO)** na sua aplicação.
- [Plataforma de identidade da Microsoft e protocolo OpenID Connect](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) - Este artigo mostra como implementar o protocolo OpenID Connect independentemente do idioma, e descreve como enviar e receber mensagens HTTP sem utilizar quaisquer bibliotecas de código aberto da Microsoft.

**Tokens de acesso**

[Tokens de acesso à plataforma de identidade da Microsoft](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) - Saiba como a sua API pode validar e utilizar as reclamações dentro de um token de acesso. Toda a documentação deste artigo, exceto quando anotado, aplica-se apenas a fichas emitidas para APIs que tenha registado. Não se aplica a fichas emitidas para APIs detidas pela Microsoft, nem esses tokens podem ser usados para validar como a plataforma de identidade da Microsoft emitirá fichas para uma API que cria.

**Configuração de aplicação**

[Redirecionar as restrições e limitações URI (URL de resposta)](https://docs.microsoft.com/azure/active-directory/develop/reply-url) - Saiba como configurar o seu URI de redirecionamento (URL de resposta). Um URI de redirecionamento, ou URL de resposta, é o local onde o servidor de autorização envia o utilizador uma vez que a aplicação foi autorizada com sucesso e concedeu um código de autorização ou ficha de acesso. O servidor de autorização envia o código ou ficha para o URI de redirecionamento; por isso é importante registar a localização correta como parte do processo de registo da aplicação.

**Provisionamento de Pedidos**

[Tutorial: Desenvolver e planear a provisão para um ponto final DO SCIM](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) - Este artigo descreve como construir um ponto final SCIM e integrar-se com o serviço de fornecimento de AAD.


