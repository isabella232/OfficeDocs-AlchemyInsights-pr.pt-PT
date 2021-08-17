---
title: Ler os registos de auditoria de eventos eliminados
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: ef4cbb0b778b22fba83d22d5056449c2281c5a2947ecb41ce8f808a4d1132426
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896026"
---
# <a name="read-the-audit-logs-for-deleted-events"></a>Ler os registos de auditoria de eventos eliminados

Eis como fazê-lo:

1. Eis uma das seguintes ações:
   - Na Centro de Conformidade do Microsoft 365 em <https://compliance.microsoft.com> , vá para Auditoria **de** \> **Soluções**. Em vez disso, para ir diretamente para **a página** Auditoria, utilize <https://compliance.microsoft.com/auditlogsearch> .
   - No portal Microsoft 365 Defender, em <https://security.microsoft.com> , vá para **Auditoria**. Em vez disso, para ir diretamente para **a página** Auditoria, utilize <https://security.microsoft.com/auditlogsearch> .

    > [!NOTE]
    > Se vir um aviso a dizer que precisa de ativar a funcionalidade, continue e ativa-a agora. Se a funcionalidade não estiver ativada, os resultados da pesquisa não poderão importar dados de datas anteriores.

2. No **separador** Procurar da **página** Auditoria, configure as seguintes definições:
   - **Intervalo de data e hora:** selecione o intervalo de data/hora nas **caixas** Início **e** Fim.
   - **Atividades:** introduza as **Exchange de caixa de correio e,** em seguida, selecione os seguintes valores:
     - **Mensagens eliminadas da pasta Itens Eliminados**
     - **Mensagens movidas para a pasta Itens Eliminados**

       Quando terminar, clique fora do painel para minimizar **o painel** Atividades.

   - **Utilizadores:** aceite o valor predefinido em branco para devolver resultados de todos os utilizadores ou introduza um ou mais utilizadores.

3. Quando terminar, clique em **Procurar**. As atividades são apresentadas na nova página **Pesquisa de** auditoria.

4. Selecione uma atividade nos resultados para abrir a panfleto de detalhes. As informações adicionais sobre o item eliminado, como o assunto da linha e a localização do item quando foi eliminado, são **apresentadas** no campoItens Afetados.

   > [!NOTE]
   > Não pode restaurar itens eliminados com a funcionalidade de registo de auditoria. Para restaurar itens eliminados, [consulte Recuperar mensagens de e-mail eliminadas Outlook na Web](https://support.microsoft.com/office/recover-deleted-email-messages-in-outlook-on-the-web-a8ca78ac-4721-4066-95dd-571842e9fb11).

Para obter mais informações, consulte [Procurar no registo de auditoria para investigar problemas de suporte comuns.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
