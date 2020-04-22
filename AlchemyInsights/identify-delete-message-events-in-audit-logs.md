---
title: Identificar eliminar eventos de mensagens em registos de auditoria
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
ms.openlocfilehash: 797a4b1146862faf91d2b9e8d74feade90f71650
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716507"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Registos de auditoria para mensagens de e-mail eliminadas

A partir de janeiro de 2019, a Microsoft está a ligar a auditoria da caixa de correio por defeito. Caso contrário, para rever apagar eventos de mensagens para um utilizador específico, tem de ativar manualmente as ações de eliminação para auditoria. Se o registo de auditoria da caixa de correio já estiver ativado para a sua organização ou para o utilizador específico, siga os passos abaixo.

1. Inicie sessão no [Microsoft 365 Security & Compliance Center](https://protection.office.com/)

2. Clique em **Procurar e Investigar** e selecione Pesquisa de Registo de **Auditoria**.

3. Selecione o intervalo de data sintetiza-se nos campos de data de **início** e data de **fim.** Especifique o nome de utilizador para o utilizador que pretende investigar (o utilizador que apagou os itens). No campo **Atividades,** selecione **Mensagens Eliminadas da pasta De itens Eliminados** e **mensagens movidas para**a pasta De itens Eliminados .

4. Clique em **Procurar**.

Nos resultados, selecione um registo de auditoria. Nos detalhes, clique em **Mais Informações.** Informações adicionais sobre o item eliminado (por exemplo, a linha de assunto e a localização do item quando foi eliminado) são apresentadas no campo **AffectedItems.** A propriedade **ClientInfoString** mostrará se a eliminação ocorreu no Outlook, Outlook na web (anteriormente conhecida como Outlook Web App), ou em qualquer outro dispositivo.

Para mais informações, consulte [Determinar quem configura o envio de e-mail para uma caixa de correio](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).

**Nota:** Não é possível recuperar itens eliminados utilizando a funcionalidade de registo de auditoria. Para recuperar mensagens eliminadas no Outlook na web, consulte ['Recuperar itens eliminados' na Aplicação Web do Outlook](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
