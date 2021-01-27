---
title: Problemas de acesso condicional
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
- "9004349"
- "7768"
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014889"
---
# <a name="conditional-access-issues"></a>Problemas de acesso condicional

**Resolver problemas com o Diagnóstico de Inscrição**

Pode rapidamente descobrir o que aconteceu ou diagnosticar problemas relacionados com o s-in do utilizador utilizando o [Diagnóstico de Inscrição:](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)

1. Lance o Diagnóstico de Inscrição.
1. Encontre o evento para analisar inserindo nos detalhes que tem sobre o utilizador, aplicação, hora de entrada, Id de pedido ou Id de correlação.
1. Reveja os resultados de diagnóstico mostrando os detalhes do que aconteceu e que ações pode tomar para fazer alterações (se forem necessárias alterações).

**Passos para resolução de problemas de um 'Sign-In'** 

1. Navegue para a página de inscrição Azure AD.
1. Filtrar as entradas pelo utilizador, intervalo de tempo, aplicação, estado, aplicação do cliente, e assim por diante.
1. Selecione um evento de inscrição e veja o separador Acesso Condicional para ver quais as políticas que foram avaliadas.
1. Clique na linha de uma política para ver os detalhes da política e entender por que se aplicou.

**Ferramentas para resolver problemas numa política de acesso condicional**

- O modo apenas de relatório permite avaliar uma política sem afetar os utilizadores.
- E se a ferramenta permite simular eventos de inscrição e ver quais as políticas que se aplicam.
- Insights e relatórios mostram o impacto em tempo real de cada política.

**Políticas de Proteção de Bases**

As políticas de proteção da linha de base foram depreciadas. Já não estão a ser aplicadas e em breve serão removidas do portal Azure. Recomendamos permitir [incumprimentos de segurança](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).

Para mais informações sobre acesso condicional consulte:

[Melhores práticas para acesso condicional no Azure Ative Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Condições de Acesso](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 Condicional [Controlos no Acesso](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 Condicional [Localizações em Acesso Condicional](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)
