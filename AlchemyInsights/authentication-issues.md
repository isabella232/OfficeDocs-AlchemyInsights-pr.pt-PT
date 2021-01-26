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
ms.openlocfilehash: 2f413e863e6aa23548e425de5901f8158e1d48ab
ms.sourcegitcommit: ba3118b7ad5e02756d0e5c2113245090f54370af
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/25/2021
ms.locfileid: "49976860"
---
# <a name="authentication-issues"></a>Problemas de autenticação

**Está à procura de informações sobre os códigos de erro AADSTS devolvidos a partir do serviço de token de segurança (STS) do Azure Active Directory (Azure AD)?** Consulte os [códigos de erro de autenticação e autorização do Azure AD](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) para localizar descrições de erros AADSTS, correções e algumas soluções sugeridas.

Os erros de autorização podem ser um resultado de vários problemas diferentes, a maioria dos quais gera um erro 401 ou 403. Por exemplo, os seguintes problemas podem causar erros de autorização:

- [Fluxos de aquisição de token de acesso](https://docs.microsoft.com/azure/active-directory/develop/authentication-vs-authorization) incorreto 
- [Âmbitos de permissão](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) mal configurados 
- Falta de [consentimento](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant#understanding-user-and-admin-consent)

Para resolver erros de autorização comuns, experimente os passos indicados abaixo que melhor se adequam ao erro que está a receber. Pode aplicar mais do que um passo para um erro que está a receber.

**401 erro Não autorizado: o seu token é válido?**

Certifique-se de que a sua aplicação está a apresentar um token de acesso válido para o Microsoft Graph como parte do pedido. Normalmente, este erro significa que o token de acesso pode estar em falta no cabeçalho do pedido de autenticação HTTP ou que o token é inválido ou expirou. Recomendamos vivamente que utilize a biblioteca de autenticação da Microsoft (MSAL) para obter aquisição de tokens de acesso. Além disso, este erro pode ocorrer se tentar utilizar um token de acesso delegado concedido a uma conta Microsoft pessoal para aceder a uma API que apenas suporta contas escolares ou profissionais (contas organizacionais).

**403 erro Proibido: selecionou o conjunto de permissões adequado?**

Certifique-se de que solicitou o conjunto de permissões correto com base nas APIs do Microsoft Graph invocadas pela sua aplicação. São fornecidas permissões com menos privilégios em todos os tópicos do método de referência da API do Microsoft Graph. Além disso, as permissões devem ser concedidas à aplicação por parte de um utilizador ou de um administrador. Normalmente, a concessão de permissões ocorre através de uma página de autorização ou da utilização do painel de registo de aplicações do portal do Azure. No painel de **Definições** para a aplicação, clique em **Permissões Necessárias** e, em seguida, em **Conceder Permissões**. Para mais informações, consulte:

- [Permissões do Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) 
- [Compreender as permissões e o consentimento do Azure AD](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)

**403 erro Proibido: a aplicação obteve um token para corresponder às permissões selecionadas?**

Certifique-se de que os tipos de permissões solicitadas ou concedidas correspondem ao tipo de token de acesso adquirido pela sua aplicação. É possível que esteja a pedir e a conceder permissões de aplicações, mas através de tokens de fluxo de código interativo delegados, em vez de tokens de fluxo de credenciais de clientes, ou a pedir e conceder permissões delegadas, mas através de tokens de fluxo de credenciais de clientes em vez de tokens de fluxo de código delegados.

Para obter mais informações relacionadas com a aquisição de tokens, consulte:

- [Obter acesso em nome dos utilizadores e permissões delegadas](https://docs.microsoft.com/graph/auth-v2-user) 
- [Azure AD v 2.0 - fluxo de código de autorização OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Obter acesso sem um utilizador (serviço daemon) e permissões de aplicação](https://docs.microsoft.com/graph/auth-v2-service) 
- [Azure AD v 2.0-fluxo de credenciais de cliente OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)

**403 erro Proibido: repor a palavra-passe**

Atualmente, não existem permissões de serviço-para-serviço daemon para permissão de aplicações que permitem repor as palavras-passe dos utilizadores. Estas APIs só são suportadas ao utilizar fluxos de código interativo delegados com um administrador com sessão iniciada. Para obter mais informações, consulte [Permissões do Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference).

**403 Proibido: o utilizador tem acesso e licença?**

Para fluxos de código delegados, o Microsoft Graph avalia se o pedido foi permitido com base nas permissões concedidas à aplicação e nas permissões que o utilizador com sessão iniciada tem. Geralmente, este erro indica que o utilizador não tem privilégios suficientes para executar o pedido **ou** que o utilizador não tem uma licença para os dados que estão a ser acedidos. Apenas os utilizadores com permissões ou licenças necessárias podem efetuar um pedido com êxito.

**403 Proibido: selecionou a API de recurso correta?**

Os serviços de API como o Microsoft Graph verificam se o pedido *aud* (audiência) no token de acesso recebido corresponde ao valor esperado para si. Caso contrário, será devolvido um erro 403 Proibido. Um procedimento incorreto que resulta neste erro é tentar utilizar um token adquirido para as APIs do Azure AD Graph, APIs do Outlook ou para as APIs do SharePoint/OneDrive para invocar o Microsoft Graph (ou vice-versa). Certifique-se de que o recurso (ou âmbito) da sua aplicação está a adquirir um token para corresponder à API que a aplicação está a invocar.

**400 Pedido Inválido ou 403 Proibido: o utilizador cumpre as políticas de acesso condicional (AC) da sua organização?**

Com base nas políticas de acesso condicional (AC) de uma organização, um utilizador que aceda aos recursos do Microsoft Graph através da sua aplicação poderá ser confrontado com a necessidade de informações adicionais que não estão presentes no token de acesso que a sua aplicação obteve originalmente. Neste caso, a sua aplicação receberá um erro **400 com *interaction_required*** durante a aquisição de token de acesso ou um erro **403 com *insufficient_claims*** ao invocar o Microsoft Graph. Em ambos os casos, a resposta de erro contém informações adicionais que podem ser apresentadas ao ponto final autorizado para pedir informações adicionais ao utilizador (como a autenticação multifator ou a inscrição de dispositivos).

Para obter mais informações relacionadas com acesso condicional, consulte:

- [Gerir os pedidos de acesso condicional através do MSAL](https://docs.microsoft.com/azure/active-directory/develop/msal-error-handling-dotnet#conditional-access-and-claims-challenges) 
- [Orientações de acesso condicional ao Azure Active Directory para programadores ](https://docs.microsoft.com/azure/active-directory/develop/v2-conditional-access-dev-guide)

**_Fim do suporte da Biblioteca de Autenticação do Active Directory (ADAL) e da API do Azure AD Graph (AAD Graph)_* _

- Desde 30 de junho de 2020, deixámos de adicionar novas funcionalidades à Biblioteca de Autenticação do Active Directory (ADAL) e à API do Azure AD Graph (AAD Graph). Continuaremos a fornecer suporte técnico e atualizações de segurança, mas deixaremos de fornecer atualizações de funcionalidades.
- A partir de 30 de junho de 2022, iremos terminar o suporte para o ADAL e para o AAD Graph e deixaremos de fornecer suporte técnico ou atualizações de segurança.
    - As aplicações que utilizam o ADAL em versões existentes do SO continuarão a funcionar após esta data mas não terão suporte técnico ou atualizações de segurança.
    - As aplicações que utilizem o AAD Graph após esta altura poderão deixar de receber respostas do ponto final do AAD Graph.

_ *Migração da ADAL**

Recomendamos que atualize para a [Biblioteca de Autenticação da Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), que tem as funcionalidades e atualizações de segurança mais recentes. Esta recomendação insere-se no contexto da migração, por parte da Microsoft, de aplicações para a MSAL na data-limite para o fim do suporte. O objetivo da migração das aplicações Microsoft para o MSAL é garantir que as aplicações beneficiam das melhorias de funcionalidades e segurança contínua da MSAL.

- [Consulte as FAQ da ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- [Saiba mais sobre como migrar aplicações por plataforma](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- Se precisar de ajuda para compreender qual das suas aplicações utiliza o ADAL, recomendamos que consulte todos os códigos de origem das aplicações e, se aplicável, contacte os fornecedores de software independentes (ISVs) ou fornecedores de aplicações. O suporte da Microsoft também pode fornecer-lhe uma lista de todas as aplicações de ADAL no seu inquilino que não sejam da Microsoft.

**Migração do AAD Graph**

Para as aplicações que utilizam o AAD Graph, siga as nossas orientações para [migrar as aplicações do Azure AD Graph para o Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist?view=graph-rest-1.0&preserve-view=true).

- [A nossa lista de verificação de migração inclui um ponto sobre introdução](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
- O portal de registo da sua aplicação Azure mostra as aplicações que estão a utilizar o AAD Graph. Recomendamos que consulte todos os códigos de origem das aplicações e, se aplicável, contacte os ISVs ou fornecedores de aplicações. O suporte da Microsoft também pode fornecer-lhe as informações sobre a toda a utilização do AAD Graph no seu inquilino.

 










