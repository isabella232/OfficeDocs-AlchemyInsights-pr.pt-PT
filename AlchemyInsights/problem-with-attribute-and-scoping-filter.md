---
title: Problema com atributo e filtro de scoping
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8470"
- "9004687"
ms.openlocfilehash: 78df24c0d8a670d678e26879cf81476f1ae9b92d
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481898"
---
# <a name="problem-with-attribute-and-scoping-filter"></a>Problema com atributo e filtro de scoping

**Problema com valores de UPN em conflito**

O Workday to AD User Provisioning Workday to AD User Provisioning mostra mensagem de erro **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**. A operação falhou porque o valor UPN previsto para a adição/modificação não é único em toda a floresta. Detalhes de erro: **CONSTRAINT_ATT_TYPE - userPrincipalName**.

O **valor do nome Do utilizadorPrincipal Que** o conector Workday está a tentar definir ao criar a conta de utilizador AD já existe no domínio de AD alvo. Isto implica que ou (1) o utilizador já existe e a verificação de identificação correspondente falhou para o utilizador ou (2) a regra de geração UPN gerou um valor conflituoso.

Aqui estão as etapas de resolução sugeridas:

Se o utilizador já existe e o controlo de identificação correspondente não conseguiu ligar a conta Workday à conta Ative Directory, verifique se o atributo ID correspondente (normalmente **funcionárioID)** em ambos os dias de trabalho e AD tem uma correspondência exata. Se não tiverem correspondência, é uma questão de dados que tem de ser corrigida. Por exemplo, se o EmployeeID no Workday for 001052 e em AD é 1052, então o motor de provisionamento não ligará as duas contas e tentará criar um utilizador que já exista. A solução neste caso é alterar o valor **do EmployeeID** em AD para incluir os principais zeros para torná-lo 001052.
Se a expressão geradora da UPN não estiver a gerar um valor único, considere usar a função de des **duplicação SelectUniqueValue** para gerar um valor único cada vez.

**O dia de trabalho para o Fornecimento de Utilizadores AD não define o valor do atributo do gestor para a conta de utilizador de AD**

O trabalho de Provisão de utilizadores de trabalho para AD não está a definir o valor do atributo **do gestor** para contas de utilizador de AD. Há dois cenários possíveis quando este comportamento é visto:

1. O gestor em Workday não pode ser resolvido para uma conta de Utilizador AD correspondente porque o gestor não está no âmbito.
2. Num cenário **de vários domínios de AD,** o gestor em Workday não está presente no mesmo domínio que o utilizador.

Experimente estes passos para resolver a questão:

1. Se tiver definido filtros de deteção, verifique primeiro se o gestor está no âmbito e se satisfaz a cláusula de deteção. Se o gestor não satisfizer o filtro de escoamento, mude o filtro de modo a que o gestor também esteja no âmbito da operação de provisionamento.
2. Se tiver vários domínios de AD, então o conector tem uma limitação conhecida da incapacidade de resolver referências de gestor de domínio transversal.

Para obter mais informações sobre a configuração do dia de trabalho para o provisionamento automatizado, consulte [Tutorial: Configure Workday para o provisionamento automático do utilizador](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).













