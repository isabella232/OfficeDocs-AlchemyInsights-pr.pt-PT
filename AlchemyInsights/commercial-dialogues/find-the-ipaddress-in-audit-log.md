---
title: Encontrar o endereço IP no registo de auditoria
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
ms.openlocfilehash: c3b1cac5379f4f3da93152fa20086068f7df562cd98b2980ce1b4280e0aa6d5f
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/11/2021
ms.locfileid: "57902271"
---
# <a name="find-the-ip-address-in-audit-log"></a>Encontrar o endereço IP no registo de auditoria

O endereço IP que corresponde a uma atividade efetuada por um utilizador ou administrador é apresentado nos registos de auditoria. As informações do cliente também são com sessão marcada. Eis como identificar o endereço IP:

1. Eis uma das seguintes ações:
   - Na Centro de Conformidade do Microsoft 365 em <https://compliance.microsoft.com> , vá para Auditoria **de** \> **Soluções**. Em vez disso, para ir diretamente para **a página** Auditoria, utilize <https://compliance.microsoft.com/auditlogsearch> .
   - No portal Microsoft 365 Defender de Equipa em <https://security.microsoft.com> , vá para **Auditoria**. Em vez disso, para ir diretamente para **a página** Auditoria, utilize <https://security.microsoft.com/auditlogsearch> .

    > [!NOTE]
    > Se vir um aviso a dizer que precisa de a ligar a auditoria, continue e a ligue-o agora. Se esta funcionalidade não estiver ativada, os resultados da pesquisa não poderão importar dados de datas anteriores.

2. Na página **Auditoria,** verifique se o separador **Procurar está** selecionado e, em seguida, configure as seguintes definições:
   - **Intervalo de data e hora:** selecione o intervalo de data/hora nas **caixas** Início **e** Fim.
   - **Atividades:** se estiver interessado numa atividade específica, selecione-a a partir da lista; caso contrário, o valor **predefinido Mostrar resultados de todas** as atividades devolve todas as atividades serão devolvidas. Tenha em atenção que determinadas atividades podem não estar disponíveis para seleção; no entanto, esses itens de auditoria serão devolvidos se **a opção Mostrar resultados de todas as atividades estiver selecionada.**
   - **Utilizadores:** aceite o valor predefinido em branco para devolver resultados de todos os utilizadores ou introduza um ou mais utilizadores.

3. Quando terminar, clique em **Procurar**. As atividades são apresentadas na nova página **Pesquisa de** auditoria.

4. Nos resultados, clique em **Filtrar Resultados** e escreva **Definir Caixa de Correio** na caixa de filtro de atividade.

5. Selecione um registo de auditoria nos resultados para abrir **a panfleto** Detalhes.

Para obter mais informações, consulte [Procurar no registo de auditoria para investigar problemas de suporte comuns.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
