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
ms.openlocfilehash: 85cbd89e461f36a51eed816619fd132ea60dfdb0014eb850c7ec3f38d41e1ca2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069975"
---
# <a name="conditional-access-issues"></a>Problemas de acesso condicional

**Resolver problemas com o Diagnóstico de Lote**

Pode descobrir rapidamente os problemas que aconteceram ou diagnosticar problemas relacionados com o iniciar trabalho do utilizador através do Diagnóstico [de Iniciar a Sua Conta:](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)

1. Inscreva o Diagnóstico de Inscrever-se.
1. Encontre o evento para analisar ao introduzir os detalhes que tem sobre o utilizador, aplicação, hora de entrada, ID do Pedido ou ID de correlação.
1. Reveja os resultados de diagnóstico que mostram os detalhes do que aconteceu e que ações pode tomar para fazer alterações (se for necessário fazer alterações).

**Passos para Remoção de um Sign-In** 

1. Navegue até à página de Assinatura do Azure AD.
1. Filtro os sign-ins por utilizador, intervalo de tempo, aplicação, estado, aplicação cliente, entre muito mais.
1. Selecione um evento de assinatura e veja o separador Acesso Condicional para ver que políticas foram avaliadas.
1. Clique na linha de uma política para ver os detalhes da política e compreender o motivo pelo qual foi aplicada.

**Ferramentas para remoção de uma política de Acesso Condicional**

- O modo só de relatório permite-lhe avaliar uma política sem afetar os utilizadores.
- A ferramenta De que se deve fazer permite-lhe simular eventos de assinatura e ver que políticas se aplicam.
- Informações e o livro de relatórios apresenta o impacto em tempo real de cada política.

**Políticas de Proteção da Linha de Base**

As políticas de Proteção do Linha Base foram pre desprotejadas. Estas deixarão de ser impossividas e serão removidas em breve do portal do Azure. Recomendamos a ativação das [predefinições de segurança.](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)

Para obter mais informações sobre o Acesso Condicional, consulte:

[Melhores práticas para acesso condicional no Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Condições no Acesso Condicional](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Controlos no Acesso Condicional](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Localizações no Acesso Condicional](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)
