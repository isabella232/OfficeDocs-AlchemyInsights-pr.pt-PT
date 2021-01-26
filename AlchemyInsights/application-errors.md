---
title: Erros de aplicação
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004342"
- "7841"
ms.openlocfilehash: 2ef90b54ce222a06740e05891fabe87b6565cb14
ms.sourcegitcommit: ba3118b7ad5e02756d0e5c2113245090f54370af
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/25/2021
ms.locfileid: "49984662"
---
# <a name="application-errors"></a>Erros de aplicação

Procurando informações sobre os códigos de **erro AADSTS** que são devolvidos do serviço de fichas de segurança Azure Ative (Azure AD) (STS)? Leia [códigos de autenticação e de erro de autorização Azure para](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) encontrar descrições de erros, correções e algumas soluções sugeridas.

Os erros de autorização podem ser resultado de vários problemas diferentes, a maioria dos quais geram um erro de 401 ou 403. Por exemplo, todos os seguintes podem levar a erros de autorização:

- Fluxos de aquisição de [fichas de acesso](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) incorretos 
- Âmbitos de [permissão](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) mal configurados 
- Falta de [consentimento](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

Para resolver erros de autorização comuns, experimente os passos abaixo que mais coincidem com o erro que está a receber. Mais de um pode aplicar-se.

**401 Erro não autorizado: O seu símbolo é válido?**

Certifique-se de que a sua aplicação está a apresentar um token de acesso válido ao Microsoft Graph como parte do pedido. Este erro significa frequentemente que o token de acesso pode estar em falta no cabeçalho de pedido autenticado HTTP ou que o token é inválido ou expirou. Recomendamos vivamente que utilize a [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) para aceder à aquisição de token. Adicionalmente, este erro pode ocorrer se tentar utilizar um token de acesso delegado concedido a uma conta pessoal da Microsoft para aceder a uma API que apenas suporta contas de trabalho ou escola (contas organizacionais).

**403 Erro Proibido: Escolheu o conjunto certo de permissões?**

Verifique se solicitou o conjunto correto de permissões com base nas APIs do Gráfico da Microsoft que a sua aplicação chama. As permissões menos privilegiadas recomendadas são fornecidas em todos os tópicos do método de referência da Microsoft Graph API. Além disso, essas permissões devem ser concedidas ao pedido por um utilizador ou administrador. A concessão de permissões normalmente acontece através de uma página de consentimento ou através da concessão de permissões utilizando a lâmina de registo de aplicações do Portal Azure. A partir da lâmina **Definições** para a aplicação, clique em **Permissões Necessárias** e, em seguida, clique em **Permissões de Concessão**.

- [Permissões de Gráfico microsoft](https://docs.microsoft.com/graph/permissions-reference) 
- [Compreender permissões e consentimento da AD Azure](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 

**403 Erro proibido: A sua aplicação adquiriu um símbolo para corresponder às permissões escolhidas?**

Certifique-se de que o tipo de permissões solicitadas ou concedidas corresponde ao tipo de sinal de acesso que a sua aplicação adquire. Pode estar a solicitar e conceder permissões de aplicação, mas usando fichas de fluxo de código interativo delegadas em vez de fichas de fluxo credenciais de clientes, ou solicitando e concedendo permissões delegadas, mas usando fichas de fluxo credenciais de cliente em vez de fichas de fluxo de código delegadas.

- [Obtenha acesso em nome dos utilizadores e permissões delegadas](https://docs.microsoft.com/graph/auth_v2_user) 
- [Azure AD v2.0 - Fluxo de código de autorização Oauth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Acesso sem um utilizador (serviço Daemon) e permissões de aplicação](https://docs.microsoft.com/graph/auth_v2_service) 
- [Azure AD v2.0 - OAuth 2.0 fluxo de credenciais de cliente](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 

**403 Erro proibido: Redefinir a palavra-passe**

Atualmente, não existem permissões de serviço-a-serviço de permissão de aplicação que permitam redefinir as palavras-passe do utilizador. Estas APIs só são suportadas utilizando os fluxos de código delegados interativos com um administrador inscrito.

- [Permissões de Gráfico microsoft](https://docs.microsoft.com/graph/permissions-reference)

**403 Proibido: O utilizador tem acesso e está licenciado?**

Para fluxos de código delegados, o Microsoft Graph avalia se o pedido é permitido com base nas permissões concedidas à app e nas permissões que o utilizador de entrada tem. Geralmente, este erro indica que o utilizador não é privilegiado o suficiente para realizar o pedido ou o utilizador não está licenciado para os dados que estão a ser acedidos. Apenas os utilizadores com as permissões ou licenças necessárias podem fazer o pedido com sucesso.

**403 Proibido: Selecionou a API de recurso correto?**

Serviços da API como o Microsoft Graph verificam se a alegação aud (audiência) no token de acesso recebido corresponde ao valor que espera para si e, se não, resulta num erro 403 Proibido. Um erro comum que resulta neste erro é tentar utilizar um símbolo adquirido para APIs, APIs do Outlook ou APIs do SharePoint/OneDrive para ligar para o Microsoft Graph (ou vice-versa). Certifique-se de que o recurso (ou âmbito) da sua aplicação está a adquirir um símbolo para corresponder à API que a aplicação está a chamar.

**400 Mau Pedido ou 403 Proibido: O utilizador cumpre as políticas de acesso condicional (CA) da sua organização?**

Com base nas políticas de CA de uma organização, um utilizador que aceda aos recursos do Microsoft Graph através da sua aplicação pode ser desafiado para obter informações adicionais que não estejam presentes no token de acesso que a sua aplicação originalmente adquirida. Neste caso, a sua aplicação recebe um 400 com um erro *de interaction_required* durante a aquisição do token de acesso ou um 403 com *insufficient_claims* erro ao ligar para o Microsoft Graph. Em ambos os casos, a resposta de erro contém informações adicionais que podem ser apresentadas ao ponto final autorizado para desafiar o utilizador para obter informações adicionais (como a autenticação de vários fatores ou a inscrição do dispositivo).

- [Tratamento de desafios de acesso condicional usando MSAL ](https://docs.microsoft.com/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
- [Orientação do desenvolvedor para acesso condicional do Azure Ative Directory](https://docs.microsoft.com/azure/active-directory/develop/conditional-access-dev-guide)
