---
title: Problemas com um diretor de recursos ou serviços
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
- "9004336"
- "7741"
ms.openlocfilehash: 9c37ad8e4dfecdb59a37d767f8eb4a5d99be7fa1
ms.sourcegitcommit: d13f23fb7994871d4e0e6e3e43672a101bd779e8
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/28/2021
ms.locfileid: "50714082"
---
# <a name="issues-with-a-resource-or-service-principal"></a>Problemas com um diretor de recursos ou serviços

1. Se está apenas a começar, [os objetos principais de aplicação e serviço no Azure Ative Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) descrevem o registo de aplicações, objetos de aplicação e diretores de serviço no Azure Ative Directory: o que são, como são usados e como estão relacionados uns com os outros. É também apresentado um cenário de exemplo multi-inquilino para ilustrar a relação entre o objeto de aplicação de uma aplicação e os objetos principais de serviço correspondentes.
2. Pode saber mais sobre a relação entre aplicações e diretores de serviços através da leitura de [aplicações e objetos principais de serviço no Azure Ative Directory.](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)
3. [Como: Utilizar o portal para criar uma aplicação AD Azure e um responsável de serviços que possa aceder](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) aos recursos mostra-lhe como criar uma nova aplicação e principal de serviço Azure Ative Que possa ser usado com o controlo de acesso baseado em funções.
4. Com a [API principal](https://docs.microsoft.com/graph/api/resources/serviceprincipal)de serviço, pode gerir programáticamente casos de aplicações e controlar o que uma aplicação pode fazer dentro do seu inquilino.
5. [serviço O tipo de recursoprincipal](https://docs.microsoft.com/graph/api/resources/serviceprincipal) lista todas as propriedades e métodos para o tipo de recurso servicePrincipal.
6. [As diferenças de tipo de recurso entre o Gráfico AD Azure e o Gráfico microsoft](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) destacam as diferenças entre os recursos AD AD do Azure e o Microsoft Graph. Mostra recursos que têm nomes diferentes ou não estão disponíveis; destaca também os recursos disponíveis na versão beta do Microsoft Graph, mas não na versão v1.0.

**Problemas com utilizadores convidados**

- [Quickstart: Adicione utilizadores convidados ao seu diretório no portal Azure](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) mostra-lhe como adicionar um novo utilizador convidado ao seu diretório AD Azure através do portal Azure, enviar um convite e ver como é o processo de resgate de convite do utilizador convidado.
- [Tutorial: Criar fluxos de utilizador no Azure Ative Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) mostra-lhe como criar alguns fluxos de utilizador recomendados utilizando o portal Azure. Se estiver à procura de informações sobre como configurar um fluxo de credenciais de senha do proprietário de recursos (ROPC) na sua aplicação, consulte configurar o fluxo de credenciais de senha do proprietário do recurso em Azure AD B2C.
