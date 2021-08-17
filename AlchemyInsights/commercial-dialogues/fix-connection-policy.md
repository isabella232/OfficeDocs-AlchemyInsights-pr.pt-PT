---
title: Corrigir política de ligação
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 9094dcdc4507f52da1dd7c95f83aa98bab1446639d2d9f52eb3a7bc849dc183c
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/11/2021
ms.locfileid: "57888417"
---
# <a name="fix-connection-policy"></a>Corrigir política de ligação

O e-mail foi marcado como seguro e entregue na Caixa de Entrada do utilizador porque o endereço IP de origem foi marcado como seguro na política de filtro de ligação predefinida. Para rever a política, faça o seguinte:

1. No portal Microsoft 365 Defender, em , vá para E-mail & políticas de <https://security.microsoft.com/>  \> **colaboração & Regras** \>  \> **contra ameaças Antisspam,** na **secção** Políticas.

   Para ir diretamente para a **página Políticas antisspam,** utilize <https://security.microsoft.com/antispam> .

2. Na página **Políticas antisspam,** selecione a política denominada Política de filtro de ligação **(Predefinição)** clicando no nome da política.

3. Na panfleto de detalhes que é exibida, clique **em Editar política de filtro de** ligação na secção **Filtragem de** ligação.

4. Reveja as **entradas** na secção Permitir sempre mensagens a partir dos seguintes endereços IP ou intervalo de endereços e veja se a opção Acionar lista **segura** está selecionada.

   > [!NOTE]
   > A Microsoft subscreve as fontes de terceiros de relevos de confiança. Se a lista de segurança estiver ativada, estes remetidos de confiança não são marcados por engano como spam. Recomendamos que selecione esta opção, uma vez que reduzirá o número de falsos positivos (e-mails bons classificados como spam) que recebe.

Para obter mais informações, consulte [Configurar a filtragem de ligações.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-connection-filter-policy)
