---
title: Problemas de autenticação
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7748"
- "9004339"
ms.openlocfilehash: 53bd0d8f8edaead519d0282239d3a6d338b297b9
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974795"
---
# <a name="authentication-issues"></a>Problemas de autenticação

**Procurando informações sobre os códigos de erro AADSTS que são devolvidos do serviço de fichas de segurança Azure Ative (Azure AD) (STS)?** Consulte [códigos de autenticação e de erro de autorização Azure para](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) encontrar descrições de erros, correções e algumas soluções de solução sugeridas.

Os erros de autorização podem ser resultado de vários problemas diferentes, a maioria dos quais geram um erro de 401 ou 403. Por exemplo, as seguintes questões podem levar a erros de autorização:

- Fluxos de aquisição de [fichas de acesso](https://docs.microsoft.com/azure/active-directory/develop/authentication-vs-authorization) incorretos 
- Âmbitos de [permissão](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) mal configurados 
- Falta de [consentimento](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant#understanding-user-and-admin-consent)

Para resolver erros de autorização comuns, experimente os passos abaixo que mais correspondam ao erro que está a receber. Mais de um passo pode aplicar-se a um erro que está a receber.

- **401 Erro não autorizado: O seu símbolo é válido?**

Certifique-se de que a sua aplicação está a apresentar um token de acesso válido ao Microsoft Graph como parte do pedido. Este erro significa frequentemente que o token de acesso pode estar em falta no cabeçalho de pedido autenticado HTTP ou que o token é inválido ou expirou. Recomendamos vivamente que utilize a Microsoft Authentication Library (MSAL) para aceder à aquisição de token. Além disso, este erro pode ocorrer se tentar utilizar um token de acesso delegado concedido a uma conta pessoal da Microsoft para aceder a uma API que apenas suporta contas de trabalho ou escola (contas organizacionais).

**403 Erro Proibido: Escolheu o conjunto certo de permissões?**

Certifique-se de que solicitou o conjunto correto de permissões com base nas APIs do Microsoft Graph que a sua aplicação chama. As permissões recomendadas com menos privilégios são fornecidas em todos os tópicos do método de referência da Microsoft Graph API. Além disso, essas permissões devem ser concedidas ao pedido por um utilizador ou administrador. A concessão de permissões ocorre normalmente através de uma página de consentimento ou utilização da lâmina de registo de aplicações do Portal Azure. A partir da lâmina **Definições** para a aplicação, clique em **Permissões Necessárias** e, em seguida, clique em **Permissões de Concessão**. Para mais informações, consulte:

- [Permissões de Gráfico microsoft](https://docs.microsoft.com/graph/permissions-reference) 
- [Compreender permissões e consentimento da AD Azure](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)

**403 Erro proibido: A sua aplicação adquiriu um símbolo para corresponder às permissões escolhidas?**

Certifique-se de que os tipos de permissões solicitadas ou concedidas correspondem ao tipo de sinal de acesso que a sua aplicação adquire. Pode estar a solicitar e conceder permissões de aplicações, mas usando fichas de fluxo de código interativo delegadas em vez de fichas de fluxo credenciais de clientes, ou solicitando e concedendo permissões delegadas, mas usando fichas de fluxo credenciais de clientes em vez de fichas de fluxo de código delegadas.

Para obter mais informações relacionadas com a aquisição de fichas, consulte:

- [Obtenha acesso em nome dos utilizadores e permissões delegadas](https://docs.microsoft.com/graph/auth-v2-user) 
- [Azure AD v2.0 - Fluxo de código de autorização Oauth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Acesso sem um utilizador (serviço Daemon) e permissões de aplicação](https://docs.microsoft.com/graph/auth-v2-service) 
- [Azure AD v2.0 - OAuth 2.0 fluxo de credenciais de cliente](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)

**403 Erro proibido: Redefinir a palavra-passe**

Atualmente, não existem permissões de serviço-a-serviço de permissão de aplicação que permitam redefinir as palavras-passe do utilizador. Estas APIs só são suportadas utilizando os fluxos de código delegados interativos com um administrador inscrito. Para obter mais informações, consulte [as permissões do Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference).

**403 Proibido: O utilizador tem acesso e está licenciado?**

Para fluxos de código delegados, o Microsoft Graph avalia se o pedido foi autorizado com base nas permissões concedidas à app e nas permissões que o utilizador de entrada tem. Geralmente, este erro indica que o utilizador não é privilegiado o suficiente para realizar o pedido **ou** o utilizador não está licenciado para os dados que estão a ser acedidos. Apenas os utilizadores com as permissões ou licenças necessárias podem fazer o pedido com sucesso.

**403 Proibido: Selecionou a API de recurso correto?**

Serviços da API como o Microsoft Graph verificam se a alegação *aud* (audiência) no token de acesso recebido corresponde ao valor que espera para si e, se não, ocorre um erro 403 Proibido. Um erro comum que resulta neste erro é tentar utilizar um símbolo adquirido para APIs, APIs do Outlook ou APIs do SharePoint/OneDrive para ligar para o Microsoft Graph (ou vice-versa). Certifique-se de que o recurso (ou âmbito) da sua aplicação está a adquirir um símbolo para corresponder à API que a aplicação está a chamar.

**400 Mau Pedido ou 403 Proibido: O utilizador cumpre as políticas de acesso condicional (CA) da sua organização?**

Com base nas políticas de acesso condicional (CA) de uma organização, um utilizador que aceda aos recursos do Microsoft Graph através da sua aplicação pode ser desafiado para obter informações adicionais que não estejam presentes no token de acesso que a sua aplicação originalmente adquirida. Neste caso, a sua aplicação recebe um **400 com um** erro de interaction_required durante a aquisição do token de acesso ou um **403 com *insufficient_claims*** erro ao ligar para o Microsoft Graph. Em ambos os casos, a resposta de erro contém informações adicionais que podem ser apresentadas ao ponto final autorizado para desafiar o utilizador para obter informações adicionais (como a autenticação de vários fatores ou a inscrição do dispositivo).

Para obter mais informações relacionadas com o acesso condicional, consulte:

- [Tratamento de desafios de acesso condicional usando MSAL](https://docs.microsoft.com/azure/active-directory/develop/msal-error-handling-dotnet#conditional-access-and-claims-challenges) 
- [Orientação do desenvolvedor para acesso condicional do Azure Ative Directory](https://docs.microsoft.com/azure/active-directory/develop/v2-conditional-access-dev-guide)

**_Fim do suporte para Azure Ative Directory Authentication Library (ADAL) e Azure AD Graph API (AAD Graph)_* _

- A partir de 30 de junho de 2020, deixaremos de adicionar quaisquer novidades à Azure Ative Directory Authentication Library (ADAL) e Azure AD Graph API (AAD Graph). Continuaremos a fornecer suporte técnico e atualizações de segurança, mas deixaremos de fornecer atualizações de funcionalidades.
- A partir de 30 de junho de 2022, terminaremos o suporte para o ADAL e a AAD Graph e deixaremos de fornecer suporte técnico ou atualizações de segurança.
    - As aplicações que utilizam o ADAL nas versões de SO existentes continuarão a funcionar após este período, mas não receberão qualquer suporte técnico ou atualizações de segurança.
    - As aplicações que utilizam o Gráfico AAD após este tempo podem deixar de receber respostas do ponto final do Gráfico AAD.

_ *Migração ADAL**

Recomendamos a atualização para a Biblioteca de Autenticação da [Microsoft (MSAL),](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)que possui as mais recentes funcionalidades e atualizações de segurança. Esta recomendação encontra-se no contexto da migração das suas aplicações para a MSAL até ao fim do prazo de suporte. O objetivo da migração de apps da Microsoft para o MSAL é garantir que as aplicações beneficiem da segurança contínua da MSAL e das melhorias de funcionalidades.

- [Leia as FAQ ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- [Saiba como migrar aplicações por plataforma](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- Se precisar de ajuda para entender quais das suas aplicações usam ADAL, recomendamos que reveja todo o código fonte das suas aplicações e, se aplicável, contacte quaisquer fornecedores de software independentes (ISV) ou fornecedores de aplicações. O suporte da Microsoft também pode fornecer-lhe uma lista de todas as aplicações ADAL não-Microsoft no seu inquilino.

**Migração de gráficos AAD**

Para aplicações que estão a usar o AAD Graph, siga a nossa orientação para [migrar aplicações AD AD para o Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist?view=graph-rest-1.0&preserve-view=true).

- [A nossa lista de verificação de migração fornece um ponto de partida.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist) 
- O portal de registo de aplicações Azure mostra quais as aplicações que estão a utilizar o AAD Graph. Recomendamos que reveja todo o código fonte das suas aplicações e, se aplicável, contacte quaisquer ISV ou fornecedores de aplicações. O suporte da Microsoft também pode fornecer-lhe a informação de todo o uso de Gráfico AAD no seu inquilino.

 










