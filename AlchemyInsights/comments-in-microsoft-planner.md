---
title: Comentários no Microsoft Planner
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001717"
- "3810"
ms.openlocfilehash: 0d87d8c9fafe49de02b9c0158144287c77339886cdb910e006296eac73a2c497
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53995518"
---
# <a name="comments-in-microsoft-planner"></a>Comentários no Microsoft Planner

Os comentários de tarefas existentes num plano são armazenados na caixa de correio do Exchange Online pertencente ao Grupo do Microsoft 365 que está associado ao plano.  Ao publicar um comentário numa tarefa, é enviada uma notificação por e-mail para a caixa de entrada do grupo. Além disso, irá receber um e-mail por cada comentário feito posteriormente na tarefa.

Seguem-se algumas respostas a problemas comuns relacionados com comentários:

- **Os utilizadores não estão a receber e-mails** – os comentários são enviados para a caixa de entrada do grupo ao qual o plano pertence. Para um utilizador receber e-mails de grupo, este último deve ser configurado de forma a enviar conversações de grupo para as caixas de entrada dos respetivos membros.

- **Os comentários não estão a ser guardados** – o utilizador que está a adicionar o comentário não tem permissão para enviar o e-mail para o grupo do Microsoft 365. Leia [Como o Microsoft Planner Funciona](https://techcommunity.microsoft.com/t5/planner-blog/how-microsoft-planner-works/ba-p/1214736) para obter mais informações sobre este cenário.

- O erro **Já não tem acesso** é apresentado ou os **utilizadores convidados não conseguem adicionar comentários** – os utilizadores convidados que não conseguem enviar um e-mail para a caixa de entrada do grupo podem ver esta mensagem. Para resolver o problema, certifique-se de que os utilizadores convidados possuem um endereço de e-mail válido.

- **Os utilizadores removidos estão a receber e-mails** – se um utilizador comentar uma tarefa antes de ter sido removido do plano, a conversação de e-mail incluirá esse utilizador em cada um dos comentários que forem feitos na tarefa.

Para obter informações detalhadas sobre comentários no Microsoft Planner, consulte [como o Microsoft Planner funciona](https://techcommunity.microsoft.com/t5/planner-blog/how-microsoft-planner-works/ba-p/1214736) e [Comentar em tarefas no Microsoft Planner](https://support.microsoft.com/office/fd4aedde-7785-4cd0-96ee-122fbc9140e1).
