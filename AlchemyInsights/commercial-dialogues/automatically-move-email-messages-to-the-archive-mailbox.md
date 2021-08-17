---
title: Mover automaticamente mensagens de e-mail para a caixa de correio de arquivo
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
- "3100008"
- "7217"
ms.openlocfilehash: 57dbfd116bbae227f2288ce23edeaaa833fadf54ca3b10b95c49512758542e32
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059237"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a>Mover automaticamente mensagens de e-mail para a caixa de correio de arquivo

Eis como configurar uma política para mover automaticamente os e-mails antigos de um utilizador para a caixa de correio de arquivo:

1. Vá para [**Arquivo &**](https://go.microsoft.com/fwlink/p/?linkid=2077143)governação dos Dados de Conformidade de Segurança para verificar se uma caixa de correio de arquivo foi  >    >   ativada para o utilizador. Se não tiver, clique em **Ativar e,** em **seguida,** clique em Sim na caixa de aviso.
2. Vá para o Exchange centro de administração [**e > de conformidade > etiquetas de retenção.**](https://go.microsoft.com/fwlink/?linkid=2059104)
3. Selecionar o ícone + e, em seguida, **selecionar aplicar automaticamente a toda a caixa de correio**.
4. Atribuir um nome à etiqueta de retenção e selecionar **Mover para o Arquivo.** Para o período de retenção, introduza o tempo que pretende, por exemplo, 90 dias. Clique em **Guardar**.
5. Agora, crie uma política de **retenção: selecionar políticas de retenção**, escolha o ícone para adicionar uma nova política.
6. Atribuir um nome à política de retenção e, em seguida, clique e desloco-se para encontrar e adicionar a etiqueta de retenção que acabou de criar. Clique em **Guardar**.
7. Por fim, aplique a política de retenção na caixa de correio do utilizador: ainda no centro de administração do Exchange, vá para **caixas** de  >  **correio dos destinatários**. Selecionar todos os utilizadores aos qual pretende aplicar a política e, em seguida, **selecionar Editar** (o ícone de lápis).
8. Na caixa de diálogo, clique em **Funcionalidades da caixa de correio.** Em **Política de retenção**, aplique a política que acabou de criar > **Guardar.**
9. Para obter instruções sobre como aplicar a política a todos os utilizadores, consulte Aplicar uma [política de retenção a caixas de correio.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
