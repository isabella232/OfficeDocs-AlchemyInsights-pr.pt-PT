---
title: Consulta da Microsoft Graph API
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004345"
- "7846"
ms.openlocfilehash: 527e88c7b3cb1cc4f5535e3b0d2bc4d8d1163336
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974682"
---
# <a name="querying-the-microsoft-graph-api"></a>Consulta da Microsoft Graph API

Este tópico também pode aplicar-se aos desenvolvedores que ainda utilizam AZure AD Graph API. No entanto, recomenda-se **vivamente** que utilize o Microsoft Graph para todos os cenários de gestão de diretórios, identidades e acessos.

**Questões de autenticação ou autorização**

- Se a sua aplicação **não conseguir adquirir fichas** para ligar para o Microsoft Graph, escolha **Problema com a obtenção de um token de acesso (Autenticação)** da categoria Microsoft Graph para obter ajuda e suporte mais específicos sobre este tópico.
- Se a sua aplicação estiver **a receber erros de autorização de 401 ou 403** ao ligar para o Microsoft Graph, escolha a categoria **API de um erro negado de acesso (Autorização)** da Microsoft para obter ajuda e suporte mais específicos sobre este tópico.

**Quero usar o Microsoft Graph, mas não sei por onde começar.**

Para saber mais sobre o Microsoft Graph, consulte:

- [Visão geral do Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Visão geral da gestão de identidade e acesso no Gráfico do Microsoft](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Começar a construir aplicativos Microsoft Graph](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** - Teste ApIs de Gráfico microsoft no seu inquilino ou inquilino de demonstração

**Quero usar o Microsoft Graph, mas suporta as APIs do diretório v1.0 que preciso?**

O Microsoft Graph é a API recomendada para a gestão de diretórios, identidades e acessos. No entanto, existem ainda algumas lacunas entre o que é possível no Azure AD Graph e microsoft Graph. Reveja os seguintes artigos, que destacam as diferenças mais atualizadas para ajudar na sua escolha:

- [Diferenças de tipo de recurso entre gráfico AD Ad Azure e Gráfico microsoft](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Diferenças de propriedade entre O Gráfico AD AZure e Gráfico microsoft](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Diferenças de método entre Azure AD e Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Quando questiono o objeto do *utilizador,* muitas das suas propriedades estão em falta**

`GET https://graph.microsoft.com/v1.0/users` apenas devolve 11 propriedades, uma vez que o Microsoft Graph seleciona automaticamente um conjunto predefinido de propriedades do *utilizador* para devolver. Se precisar de outras propriedades *do utilizador,* utilize $select para escolher as propriedades de que a sua aplicação necessita. Experimente primeiro no **Microsoft Graph Explorer.**

**Alguns valores de propriedade do utilizador são *nulos,* embora eu saiba que estão definidos**

A explicação mais provável é que o pedido tinha sido concedido à permissão *User.ReadBasic.All.* Isto permite que a aplicação leia um conjunto limitado de propriedades do utilizador, devolvendo todas as outras propriedades como nulas, mesmo que tenham sido previamente definidas. Tente conceder a aplicação *User.Read.All* permission in instead.

Para obter mais informações, consulte [as permissões do utilizador do Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference#user-permissions).

**Estou com dificuldade em usar parâmetros de consulta OData para filtrar dados nos meus pedidos**

Embora o Microsoft Graph suporte uma vasta gama de parâmetros de consulta OData, muitos desses parâmetros não são totalmente suportados por serviços de diretório (recursos que herdam do *directórioObject)* no Microsoft Graph. As mesmas limitações que estavam presentes no Azure AD Graph persistem na maior parte do Microsoft Graph:

1. **Não apoiado:**$count, $search e $filter em *valores nulos* ou *não nulos*
2. **Não suportado**: $filter sobre determinadas propriedades (ver tópicos de recursos sobre os quais as propriedades são filtradas)
3. **Não suportado:** paging, filtragem e triagem ao mesmo tempo
4. **Não suportado:** filtrar uma relação. Por exemplo - encontre todos os membros do grupo de engenharia que estão no Reino Unido.
5. **Suporte parcial**: $orderby no *utilizador* (só no nome do utilizador e no userPrincipalName) e *no grupo*
6. **Suporte parcial**: $filter (suporta apenas *o suporte eq*, começa *com*, *ou*, *e* limitou *qualquer suporte*) $expand (expandir as relações de um único objeto devolve todas as relações, mas expandir uma coleção de relacionamentos de objetos é limitada)

Para obter mais informações, consulte [Personalizar respostas com parâmetros de consulta.](https://docs.microsoft.com/graph/query-parameters)

**A API que estou a ligar não funciona, onde posso fazer mais testes?**

**Microsoft Graph Explorer** - Teste APIs do Microsoft Graph no seu inquilino ou inquilino de demonstração e também confira as consultas de **amostra** no Microsoft Graph Explorer.

**Quando faço perguntas sobre dados, parece que recebo um conjunto de dados incompleto**

Se estiver a consultar uma coleção (como *utilizadores),* o Microsoft Graph utiliza os limites da página do lado do servidor para que os resultados sejam sempre devolvidos com um tamanho de página padrão. A sua aplicação deve sempre esperar página através de coleções devolvidas do serviço.

Para mais informações, consulte:

- [As melhores práticas do Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [Paging dados do Microsoft Graph na sua app](https://docs.microsoft.com/graph/paging)

**A minha aplicação é muito lenta e também está a ser estrangulada. Que melhorias posso fazer?**

Dependendo do seu cenário, existem várias opções à sua disposição para tornar a sua aplicação mais performante e, em alguns casos, menos propensa a ser estrangulada pelo serviço (quando está a fazer demasiadas chamadas).

Para saber mais informações, consulte os artigos:

- [As melhores práticas do Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [Pedidos de loteamento](https://docs.microsoft.com/graph/json-batching)
- [Mudanças de faixa através da consulta delta](https://docs.microsoft.com/graph/delta-query-overview)
- [Ser notificado das alterações através de webhooks](https://docs.microsoft.com/graph/webhooks)
- [Orientação de estrangulamento](https://docs.microsoft.com/graph/throttling)

**Onde posso encontrar mais informações sobre erros e questões conhecidas?**

- [Informações de resposta a erros do Microsoft Graph](https://docs.microsoft.com/graph/errors)
- [Problemas conhecidos com o Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**Onde posso verificar o estado da disponibilidade de serviço e conectividade?**

A disponibilidade de serviço e conectividade dos serviços subjacentes que podem ser acedidos através do Microsoft Graph podem ter impacto na disponibilidade e desempenho globais do Microsoft Graph.

- Para a saúde do serviço de diretório ativo Azure, verifique o estado dos serviços de **Segurança + Identidade** listados na página de estado do [Azure](https://azure.microsoft.com/status/).
- Para os serviços do Office que contribuem para o Microsoft Graph, verifique o estado dos serviços listados no [Painel de Saúde do Office Service](https://portal.office.com/adminportal/home#/servicehealth).
