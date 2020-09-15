---
title: Identificar endereço IP e cliente em registos de auditoria
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 295418f3c433df2ba1004f4bec4377c68e6bb155
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668321"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Identificar endereço IP e cliente em registos de auditoria

O endereço IP que corresponde a uma atividade de um utilizador ou administrador microsoft 365 é mostrado nos Registos de Auditoria. A informação do cliente também está registada. Aqui estão os passos para identificar tais informações

1. Faça login no [Microsoft 365 Security & Compliance Center](https://protection.office.com/).

2. Aceda à página de pesquisa de registo de registo de auditoria **de pesquisa.**  >  **Audit log search**

   Se estiver interessado numa atividade específica, selecione-a da lista **de Atividades.** Caso contrário, todas as atividades serão devolvidas para o utilizador selecionado (definição predefinição).

   **Nota:** Certas atividades podem não estar disponíveis no menu **Atividades;** no entanto, esses itens de auditoria serão devolvidos se **os Resultados do Show para todas as atividades** forem selecionados (definição predefinida).

3. Especifique o nome de utilizador no campo **Utilizadores,** selecione o intervalo de datas apropriado para a atividade e, em seguida, clique em **Procurar**.

Nos resultados, pode ver o endereço IP para essa atividade no painel de resultados. Selecione o registo de auditoria para ver informações **detalhadas** no flyout Details (por exemplo, Cliente, Utilizador que realizou ação, etc.).

Para obter mais informações, consulte [encontrar o endereço IP do computador utilizado para aceder a uma conta comprometida.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account)
