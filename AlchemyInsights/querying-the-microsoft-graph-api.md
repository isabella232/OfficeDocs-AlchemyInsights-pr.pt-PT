---
title: Consulta na API de Graph Microsoft
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
ms.openlocfilehash: eda5d8d1d76d0d87312b1441aeae89d8e250abe0e8b613d4a43fcc2345a6f021
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923250"
---
# <a name="querying-the-microsoft-graph-api"></a>Consulta na API de Graph Microsoft

Este tópico também pode aplicar-se aos programadores que ainda utilizam a Azure AD Graph API. No entanto, **recomendamos vivamente que** utilize o Microsoft Graph para todos os cenários de gestão de diretórios, identidades e acesso.

**Problemas de autenticação ou autorização**

- Se a sua aplicação não conseguir adquirir **tokens** para ligar para o Microsoft Graph, escolha Problema ao obter uma categoria de **token** de acesso (Autenticação) do Microsoft Graph para obter ajuda e suporte mais específicos sobre este tópico.
- Se a sua aplicação estiver a receber erros de autorização **401 ou 403** ao ligar para o Microsoft Graph, escolha a categoria Obter um erro de acesso negado **(Autorização)** da API do Microsoft Graph para obter ajuda e suporte mais específicos sobre este tópico.

**Quero utilizar o Microsoft Graph, mas não tenho a certeza por onde começar**

Para saber mais sobre o Microsoft Graph, consulte:

- [Visão geral do Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Overview of Identity and Access Management in Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Começar a criar aplicações microsoft Graph Microsoft](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer -** Teste as APIs do Microsoft Graph no seu inquilino ou um inquilino de demonstração

**Quero utilizar o Microsoft Graph, mas suporta as APIs do diretório v1.0 de que preciso?**

O Microsoft Graph é a API recomendada para a gestão de diretórios, identidades e acessos. No entanto, ainda existem alguns intervalos entre o que é possível fazer no Azure AD Graph Microsoft Graph. Reveja os seguintes artigos, que destacam as diferenças mais recentes para ajudar na sua escolha:

- [Diferenças de tipo de recurso entre o Azure AD Graph e o Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Diferenças de propriedades entre o Azure AD Graph e o Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Diferenças de métodos entre o Azure AD e o Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Quando consulta o objeto do *utilizador,* muitas das suas propriedades estão em falta**

`GET https://graph.microsoft.com/v1.0/users`devolve apenas 11 propriedades, uma vez que o Microsoft Graph seleciona automaticamente um conjunto predefinido de *propriedades* de utilizador a devolver. Se precisar de outras *propriedades de* utilizador, utilize o $select para escolher as propriedades de que a sua aplicação necessita. Experimente primeiro no **Microsoft Graph Explorer.**

**Alguns valores de propriedade do utilizador são *nulos apesar* de saber que estão definidos**

A explicação mais provável é que a aplicação tenha sido concedida à *permissão User.ReadBasic.All.* Isto permite que a aplicação leia um conjunto limitado de propriedades de utilizador, devolvendo todas as outras propriedades como nulos, mesmo que tenham sido definidas anteriormente. Em alternativa, experimente conceder *a permissão User.Read.All* à aplicação.

Para obter mais informações, consulte [Microsoft Graph permissões de utilizador.](https://docs.microsoft.com/graph/permissions-reference#user-permissions)

**Estou a ter problemas ao utilizar parâmetros de consulta OData para filtrar dados nos meus pedidos**

Embora o Microsoft Graph suporte uma grande variedade de parâmetros de consulta de OData, muitos desses parâmetros não são totalmente suportados pelos serviços de diretório (recursos que herdam do *diretórioObject)* no Microsoft Graph. As mesmas limitações que estavam presentes no Azure AD Graph persistem na maioria das ações no Microsoft Graph:

1. **Não suportado:**$count, $search e $filter valores *nulos* ou *não nulos*
2. **Não suportado:**$filter sobre determinadas propriedades (consulte tópicos de recursos sobre as quais as propriedades podem ser filtradas)
3. **Não suportado:** paging, filtragem e ordenação ao mesmo tempo
4. **Não suportado:** filtragem numa relação. Por exemplo, encontre todos os membros do grupo de engenharia que estão no Reino Unido.
5. **Suporte parcial:**$orderby *utilizador* (apenas displayName e userPrincipalName) e *grupo*
6. Suporte **parcial:**$filter (suporta apenas *eq,* começa *com* *,* ou *,* e , e limitado *qualquer*) suporte, $expand (expandir as relações de um único objeto devolve todas as relações, mas expandir uma coleção de relações de objetos é limitado)

Para obter mais informações, [consulte Personalizar respostas com parâmetros de consulta.](https://docs.microsoft.com/graph/query-parameters)

**A API para a qual estou a ligar não funciona. Onde posso fazer mais testes?**

**Microsoft Graph Explorer** - Teste as APIs do Microsoft Graph no seu inquilino  ou um inquilino de demonstração e consulte também as consultas de exemplo no Microsoft Graph Explorer.

**Quando consultai dados, parece que receba um conjunto de dados incompleto**

Se estiver a fazer consultas a uma coleção (como *utilizadores),* o Microsoft Graph utiliza limites de página do lado do servidor para que os resultados sejam sempre devolvidos com um tamanho de página predefinido. A sua aplicação deve esperar sempre que esprepar as coleções devolvidas do serviço.

Para mais informações, consulte:

- [Melhores Graph Microsoft](https://docs.microsoft.com/graph/best-practices-concept)
- [Paging Microsoft Graph dados na sua aplicação](https://docs.microsoft.com/graph/paging)

**A minha aplicação é demasiado lenta e também está a ser pequena. Que melhorias posso fazer?**

Dependendo do seu cenário, existem à sua disposição várias opções diferentes para tornar a sua aplicação mais eficaz e, em alguns casos, menos probabilidade de ser refletida pelo serviço (quando faz demasiadas chamadas).

Para saber mais informações, consulte os artigos:

- [Melhores Graph Microsoft](https://docs.microsoft.com/graph/best-practices-concept)
- [Pedidos de lote](https://docs.microsoft.com/graph/json-batching)
- [Controlar alterações através de uma consulta delta](https://docs.microsoft.com/graph/delta-query-overview)
- [Receber notificações de alterações através de Webhooks](https://docs.microsoft.com/graph/webhooks)
- [Orientação da ressarceção de ajuda](https://docs.microsoft.com/graph/throttling)

**Onde posso encontrar mais informações sobre erros e problemas conhecidos?**

- [Informação Graph resposta a erros do Microsoft Graph Microsoft](https://docs.microsoft.com/graph/errors)
- [Problemas conhecidos do Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**Onde posso verificar o estado da disponibilidade do serviço e da conectividade?**

A disponibilidade do serviço e a conectividade dos serviços submetidos que podem ser acededos através do Microsoft Graph pode afetar a disponibilidade geral e o desempenho do Microsoft Graph.

- Para Azure Active Directory estado de serviço, verifique o estado dos serviços **de Segurança e Identidade** listados na página de estado do [Azure.](https://azure.microsoft.com/status/)
- Para Office serviços que contribuem para o Microsoft Graph, verifique o estado dos serviços listados [no Dashboard](https://portal.office.com/adminportal/home#/servicehealth)Office Estado de Serviço.
