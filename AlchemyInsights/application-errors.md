---
title: Erros da aplicação
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
ms.openlocfilehash: ce4c89da79112726ed4fb25527edc8d082bd37f239595b9eab7279abeeecfd7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53931460"
---
# <a name="application-errors"></a>Erros da aplicação

Está à procura de informações sobre os códigos de erro **do AADSTS** que são devolvidos do serviço de tokens de segurança (STS) do Azure Active Directory (Azure AD)? Leia Códigos de erro de autenticação e autorização do [Azure AD](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) para encontrar descrições de erros, correções e algumas sões sugeridas do AADSTS.

Os erros de autorização podem ser um resultado de vários problemas diferentes, a maioria dos quais gera um erro 401 ou 403. Por exemplo, o seguinte pode levar a erros de autorização:

- [Fluxos de aquisição de token de acesso](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) incorreto 
- [Âmbitos de permissão](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) mal configurados 
- Falta de [consentimento](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

Para resolver erros de autorização comuns, experimente os passos fornecidos abaixo que melhor correspondem ao erro que está a receber. Pode aplicar-se mais do que um.

**401 erro Não autorizado: o seu token é válido?**

Certifique-se de que a sua aplicação está a apresentar um token de acesso válido ao Microsoft Graph como parte do pedido. Normalmente, este erro significa que o token de acesso pode estar em falta no cabeçalho do pedido de autenticação HTTP ou que o token é inválido ou expirou. Recomendamos vivamente que utilize a [Microsoft Authentication Library (MSAL) para aquisição](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) de tokens de acesso. Além disso, este erro pode ocorrer se tentar utilizar um token de acesso delegado concedido a uma conta Microsoft pessoal para aceder a uma API que apenas suporta contas escolares ou profissionals (contas organizacionais).

**403 erro Proibido: selecionou o conjunto de permissões adequado?**

Verifique se pediu o conjunto correto de permissões com base nas APIs de permissões do Microsoft Graph as suas chamadas de aplicação. As permissões menos privilegiadas recomendadas são fornecidas em todos os tópicos de referência da API Graph Microsoft Graph. Além disso, as permissões devem ser concedidas à aplicação por parte de um utilizador ou de um administrador. Normalmente, a concessão de permissões ocorre através de uma página de consentimento ou ao conceder permissões através da folha de registo da aplicação Portal do Azure. No painel de **Definições** para a aplicação, clique em **Permissões Necessárias** e, em seguida, em **Conceder Permissões**.

- [Permissões do Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) 
- [Compreender as permissões e o consentimento do Azure AD](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 

**403 erro Proibido: a aplicação obteve um token para corresponder às permissões selecionadas?**

Certifique-se de que o tipo de permissões pedidas ou concedidas corresponde ao tipo de token de acesso que a sua aplicação adquire. Poderá estar a pedir e a conceder permissões de aplicações, mas a utilizar tokens de fluxo de código interativo delegado em vez de tokens de fluxo de credenciais de cliente ou a pedir e conceder permissões delegadas, mas utilizar tokens de fluxo de credenciais de cliente em vez de tokens de fluxo de código delegado.

- [Obter acesso em nome dos utilizadores e permissões delegadas](https://docs.microsoft.com/graph/auth_v2_user) 
- [Azure AD v 2.0 - fluxo de código de autorização OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Obter acesso sem um utilizador (serviço daemon) e permissões de aplicação](https://docs.microsoft.com/graph/auth_v2_service) 
- [Azure AD v 2.0-fluxo de credenciais de cliente OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 

**403 erro Proibido: repor a palavra-passe**

Atualmente, não existem permissões de serviço-para-serviço daemon para permissão de aplicações que permitem repor as palavras-passe dos utilizadores. Estas APIs só são suportadas ao utilizar fluxos de código interativo delegados com um administrador com sessão iniciada.

- [Permissões do Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference)

**403 Proibido: o utilizador tem acesso e licença?**

Para fluxos de código delegados, o Microsoft Graph avalia se o pedido é permitido com base nas permissões concedidas à aplicação e nas permissões que o utilizador com assinatura assinada tem. Geralmente, este erro indica que o utilizador não tem privilégios suficientes para executar o pedido ou que o utilizador não tem uma licença para os dados que estão a ser acedidos. Apenas os utilizadores com permissões ou licenças necessárias podem efetuar um pedido com êxito.

**403 Proibido: selecionou a API de recurso correta?**

Serviços da API, como o Microsoft Graph, verificam que o pedido de AUD (audiência) no token de acesso recebido corresponde ao valor esperado para si próprio e, caso não se verifique, resulta num erro Proibido 403. Um procedimento incorreto que resulta neste erro é tentar utilizar um token adquirido para as APIs do Azure AD Graph, APIs do Outlook ou para as APIs do SharePoint/OneDrive para invocar o Microsoft Graph (ou vice-versa). Certifique-se de que o recurso (ou âmbito) da sua aplicação está a adquirir um token para corresponder à API que a aplicação está a invocar.

**400 Pedido Inválido ou 403 Proibido: o utilizador cumpre as políticas de acesso condicional (AC) da sua organização?**

Com base nas políticas de AC de uma organização, o acesso original de um utilizador aos recursos do Microsoft Graph através da sua aplicação poderá ser desafiado para obter informações adicionais que não estão presentes no token de acesso que a sua aplicação adquiriu originalmente. Neste caso, a sua aplicação receberá um erro 400 com *interaction_required* durante a aquisição de token de acesso ou um erro 403 com *insufficient_claims* ao invocar o Microsoft Graph. Em ambos os casos, a resposta ao erro contém informações adicionais que podem ser apresentadas no ponto final de autorização para contestar o utilizador para obter informações adicionais (como a autenticação multifatores ou a inscrição de dispositivos).

- [Lidar com desafios de acesso condicional utilizando MSAL ](https://docs.microsoft.com/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
- [Orientações de acesso condicional ao Azure Active Directory para programadores ](https://docs.microsoft.com/azure/active-directory/develop/conditional-access-dev-guide)
