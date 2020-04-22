---
title: Identificar endereço IP e cliente em registos de auditoria
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: d1a0d412fc0c6d79e50b101ca759127522f45dcd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716399"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Identificar endereço IP e cliente em registos de auditoria

O endereço IP que corresponde a uma atividade de um utilizador ou administrador da Microsoft 365 é mostrado nos Registos de Auditoria. A informação do cliente também está registada. Aqui estão os passos para identificar tais informações

1. Inicie sessão no [Microsoft 365 Security & Compliance Center](https://protection.office.com/).

2. Aceda à página de pesquisa de registo de auditoria de > **pesquisa.** **Search**

   Se estiver interessado numa atividade específica, selecione-a na lista de **Atividades.** Caso contrário, todas as atividades serão devolvidas para o utilizador selecionado (definição predefinida).

   **Nota:** Determinadas atividades podem não estar disponíveis no menu **Atividades;** no entanto, esses itens de auditoria serão devolvidos se os **Resultados do Espetáculo para todas as atividades** forem selecionados (definição padrão).

3. Especifique o nome de utilizador no campo **Utilizadores,** selecione a gama de datas apropriada para a atividade e, em seguida, clique em **Procurar**.

Nos resultados, pode ver o endereço IP para essa atividade no painel de resultados. Selecione o registo de auditoria para ver informações detalhadas no flyout **de Detalhes** (por exemplo, Cliente, Utilizador que realizou ação, etc.).

Para mais informações, consulte [Encontrar o endereço IP do computador utilizado para aceder a uma conta comprometida](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).
