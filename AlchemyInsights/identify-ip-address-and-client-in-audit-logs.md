---
title: Identificar o endereço IP e o cliente nos registos de auditoria
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: e0119762d2a34bd2b0da827faf55c832e29d8a2b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539040"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Identificar o endereço IP e o cliente nos registos de auditoria

O endereço IP que corresponde a uma actividade por um utilizador do Office 365 ou o administrador é mostrado nos registos de auditoria. As informações de cliente também estão registadas. Eis os passos para identificar essas informações

1. Inicie sessão para o [Centro de conformidade do Office 365 segurança &](https://protection.office.com/).

2. Vá para a **pesquisa**de > página de**procura de registo de auditoria** .

   Se estiver interessado numa actividade específica, seleccione-a lista de **actividades** . Caso contrário, todas as actividades serão devolvidas para o utilizador seleccionado (predefinição).

   **Nota**: certas actividades podem não estar disponíveis no menu de **actividades** ; No entanto, os itens de auditoria será devolvido se **Mostrar os resultados para todas as actividades** é seleccionada (predefinição).

3. Especificar o nome de utilizador no campo **utilizadores** , seleccione o intervalo de data apropriada para a actividade e, em seguida, clique em **Procurar**.

Os resultados, pode ver o endereço IP para essa actividade no painel de resultados. Seleccione o registo de auditoria para ver informações detalhadas na lista de opções **Detalhes** (por exemplo, cliente, utilizador que executou a acção, etc.).

Para mais informações, consulte a [localização do endereço IP do computador utilizado para aceder a uma conta comprometida](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).
