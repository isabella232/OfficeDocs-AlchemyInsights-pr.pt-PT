---
title: Comentários em Itens de lista
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003821"
- "6841"
ms.openlocfilehash: d72e3de6da9f51ebd5dd8a4eb06e94d7bc5cca81f86bd61902a9587b00f7b7b0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53995498"
---
# <a name="comments-on-list-items"></a>Comentários em Itens de lista

Os utilizadores podem ver todos os comentários num item de lista e filtrar entre vistas que mostram comentários ou atividade relacionada com um item.

Os utilizadores têm de ter em atenção o seguinte antes de podeem adicionar e eliminar comentários:

- Os comentários seguem as definições de permissão inerentes no SharePoint.
- As listas clássicas que ainda não foram criadas para aparecer em interfaces de utilizador modernas, como listas de tarefas, não terão esta funcionalidade de comentários.
- Comentar em listas no Teams não está disponível nesta versão.
- Os comentários não são indexados pela Pesquisa.

Os administradores podem desativar esta funcionalidade ao nível da organização ao alterar o parâmetro **CommentsOnListItemsDisabled** no cmdlet **Set-SPOTenant** PowerShell.

Atualmente, não é possível desativar o comentário ao nível do site ou da lista. Esperamos ter esses controlos numa atualização posterior, provavelmente no primeiro trimestre de 2021.
