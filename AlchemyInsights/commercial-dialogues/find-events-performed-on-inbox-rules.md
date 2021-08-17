---
title: Encontrar eventos efetuado em regras de caixa de entrada
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
ms.openlocfilehash: 626bd7515270f03e1560a3ed637e7bc60b374c5525527205d5f6775e4758f07a
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/11/2021
ms.locfileid: "57882646"
---
# <a name="find-events-performed-on-inbox-rules"></a>Encontrar eventos efetuado em regras de caixa de entrada

Quando as regras de caixa de entrada são criadas, alteradas ou eliminadas, os eventos são registados no registo de auditoria. Eis como revê-los:

1. Eis uma das seguintes ações:
   - Na Centro de Conformidade do Microsoft 365 em <https://compliance.microsoft.com> , vá para Auditoria **de** \> **Soluções**. Em vez disso, para ir diretamente para **a página** Auditoria, utilize <https://compliance.microsoft.com/auditlogsearch> .
   - No portal Microsoft 365 Defender, em <https://security.microsoft.com> , vá para **Auditoria**. Em vez disso, para ir diretamente para **a página** Auditoria, utilize <https://security.microsoft.com/auditlogsearch> .

    > [!NOTE]
    > Se vir um aviso a dizer que precisa de a ligar a auditoria, continue e a ligue-o agora. Se esta funcionalidade não estiver ativada, os resultados da pesquisa não poderão importar dados de datas anteriores.

2. No **separador** Procurar da **página** Auditoria, configure as seguintes definições:
   - **Intervalo de data e hora:** selecione o intervalo de data/hora nas **caixas** Início **e** Fim.
   - **Atividades: selecione** **Nova Caixa de EntradaRule Criar regra de caixa de entrada a partir Outlook Web App**

3. Quando terminar, clique em **Procurar**. As atividades são apresentadas na nova página **Pesquisa de** auditoria.

4. Selecione uma atividade nos resultados para abrir a panfleto de detalhes. Na secção **Parâmetros,** pode ver o nome da regra, o conjunto de condições e as ações que a regra irá tomar.

Para saber mais, consulte Procurar [no registo de auditoria para investigar problemas de suporte comuns.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
