---
title: Identificar o endereço IP e o cliente nos registos de auditoria
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
ms.openlocfilehash: fcad71bcc5ea6036bc8fa25a9be38caabc4d0889ee01ea86e23065333d5fce0a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54014911"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Identificar o endereço IP e o cliente nos registos de auditoria

O endereço IP que corresponde a uma atividade por um Microsoft 365 ou administrador é apresentado nos Registos de Auditoria. As informações do cliente também são com sessão marcada. Eis os passos para identificar essas informações

1. In iniciar sessão no [Centro Microsoft 365 conformidade.](https://protection.office.com/)

2. Aceda à página **Pesquisa de registo** de auditoria  >  **de** pesquisa.

   Se estiver interessado numa atividade específica, selecione-a na **lista Atividades.** Caso não o esteja a fazer, todas as atividades serão devolvidas para o utilizador selecionado (predefinição).

   **Nota:** determinadas atividades podem não estar disponíveis **no** menu Atividades; no entanto, esses itens de auditoria serão devolvidos se a **opção Mostrar Resultados de todas as atividades estiver selecionada** (predefinição).

3. Especifique o nome de utilizador no campo **Utilizadores,** selecione o intervalo de datas adequado para a atividade e, em seguida, clique em **Procurar**.

Nos resultados, pode ver o endereço IP para essa atividade no painel de resultados. Selecione o registo de  auditoria para ver informações detalhadas na lista de folheto Detalhes (por exemplo, Cliente, Utilizador que efetuou ação, etc.).

Para obter mais informações, consulte [Encontrar o endereço IP do computador utilizado para aceder a uma conta comprometida.](/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account)
