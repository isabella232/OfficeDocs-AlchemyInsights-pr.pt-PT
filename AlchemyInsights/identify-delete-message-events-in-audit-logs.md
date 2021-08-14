---
title: Identificar eventos de eliminação de mensagens em registos de auditoria
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
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: f68b623abd0efa990df71e5bf1ea1c9e7367ed691b1752f68c971e973922a63d
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/11/2021
ms.locfileid: "57868429"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Auditar registos de mensagens de e-mail eliminadas

A partir de janeiro de 2019, a Microsoft atale o registo de auditoria de caixa de correio por predefinição. Caso contrário, para rever os eventos de eliminação de mensagens de um utilizador específico, tem de ativar manualmente as ações de eliminação para auditoria. Se o registo de auditoria de caixa de correio já estiver ativado para a sua organização ou para o utilizador específico, siga os passos abaixo.

1. Iniciar sessão no Centro [Microsoft 365 conformidade](https://protection.office.com/)

2. Clique em **Pesquisa e Investigação e selecione** Pesquisa de Registo de **Auditoria**.

3. Selecione o intervalo de **datas nos campos Data de início** e Data **de** fim. Especifique o nome de utilizador do utilizador que pretende investigar (o utilizador que eliminou os itens). No campo **Atividades, selecione** **Mensagens** eliminadas da pasta Itens Eliminados e Mensagens movidas para a **pasta Itens Eliminados**.

4. Clique **em Procurar**.

Nos resultados, selecione um registo de auditoria. Na panfleto de detalhes, clique **em Mais Informações.** As informações adicionais sobre o item eliminado (por exemplo, o assunto da linha e a localização do item quando foi eliminado) são **apresentadas** no campoItens Afetados. A **propriedade ClientInfoString** será mostrada se a eliminação ocorreu no Outlook, Outlook na Web (anteriormente conhecido como Outlook Web App) ou em qualquer outro dispositivo.

Para obter mais informações, consulte Determinar [quem configurar o receção de e-mails para uma caixa de correio.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items)

**Nota:** não pode obter itens eliminados com a funcionalidade de registo de auditoria. Para obter mensagens eliminadas no Outlook na Web, consulte Recuperar [itens eliminados no Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
