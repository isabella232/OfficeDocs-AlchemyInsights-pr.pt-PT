---
title: Identificar excluir eventos de mensagens em registos de auditoria
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 641c0216491186aeb423a13854c6b39ee005e5df
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508999"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Registos de auditoria para mensagens de correio de correio de correio apagados

A partir de janeiro de 2019, a Microsoft está a ligar a auditoria da caixa de correio por padrão. Caso contrário, para rever os eventos de mensagens para um utilizador específico, é necessário ativar manualmente as ações de eliminação para auditoria. Se o registo de auditoria da caixa de correio já estiver ativado para a sua organização ou para o utilizador específico, siga os passos abaixo.

1. Faça login no [Microsoft 365 Security & Compliance Center](https://protection.office.com/)

2. Clique em **Pesquisar e Investigar** e selecione Audit Log **Search**.

3. Selecione o intervalo de datas nos campos **data de início** e **fim.** Especifique o nome de utilizador para o utilizador que pretende investigar (o utilizador que eliminou os itens). No campo **Atividades,** **selecione mensagens eliminadas da pasta de itens eliminados** e **mensagens movidas para pasta de Itens Eliminados**.

4. Clique **em Pesquisar**.

Nos resultados, selecione um registo de auditoria. No voo de informação, clique em **Mais Informações.** Informações adicionais sobre o item eliminado (por exemplo, a linha de assunto e a localização do item quando foi eliminado) são apresentadas no campo **AffectedItems.** A propriedade **ClientInfoString** mostrará se a eliminação ocorreu no Outlook, Outlook na web (anteriormente conhecida como Outlook Web App), ou qualquer outro dispositivo.

Para obter mais informações, consulte [Determineing quem criou o reencaminhamento de e-mail para uma caixa de correio](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).

**Nota:** Não é possível recuperar itens eliminados utilizando a função de registo de auditoria. Para obter mensagens eliminadas no Outlook na web, consulte [Recuperar itens eliminados na App Web do Outlook](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
