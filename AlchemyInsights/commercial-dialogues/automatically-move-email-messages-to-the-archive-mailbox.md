---
title: Mover automaticamente mensagens de correio eletrónico para a caixa de correio de arquivo
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
ms.openlocfilehash: 14ded561ee2b3c244fadbdab42fd0e833a1c66d5
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749285"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a>Mover automaticamente mensagens de correio eletrónico para a caixa de correio de arquivo

Eis como configurar uma política para mover automaticamente o antigo e-mail de um utilizador para a caixa de correio de arquivo:

1. Vá ao [**Security & Compliance**](https://go.microsoft.com/fwlink/p/?linkid=2077143)Data Governance Archive para verificar se uma caixa de correio de arquivo foi  >    >   ativada para o utilizador. Se não tiver, clique em **Ativar** então **Sim** na caixa de aviso.
2. Vá ao [**Centro de Administração Exchange > etiquetas de gestão de conformidade > de retenção.**](https://go.microsoft.com/fwlink/?linkid=2059104)
3. Escolha o ícone + e escolha **aplicar-se automaticamente a toda a caixa de correio.**
4. Atribua um nome à etiqueta de retenção e escolha **Mover to Archive**. Para o período de retenção, insira o tempo que quiser, como 90 dias. Clique em **Guardar**.
5. Agora crie uma política de retenção: escolha **políticas de retenção,** escolha o ícone para adicionar uma nova política.
6. Atribua um nome à política de retenção, clique e percorra para encontrar e adicionar a etiqueta de retenção que acabou de criar. Clique em **Guardar**.
7. Por fim, aplique a política de retenção na caixa de correio do utilizador: ainda no centro de administração Exchange, vá às caixas de correio **dos**  >  **destinatários**. Escolha todos os utilizadores a quem pretende aplicar a política e, em seguida, escolha **Editar** (o ícone do lápis).
8. Na caixa de diálogo, clique nas **funcionalidades da caixa de correio**. No âmbito **da política de retenção,** aplique a política que acabou de criar > **Salvar**.
9. Para obter instruções para aplicar a apólice a todos os utilizadores, consulte [Aplicar uma política de retenção nas caixas de correio](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).
