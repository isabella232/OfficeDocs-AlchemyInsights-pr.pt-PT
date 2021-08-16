---
title: As Políticas de Retenção Exchange Centro de Administração não funcionam
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 6652ad5fc1691e1d5a4293d81f3a649f23ec38f18c8ed9fe06665628a901d13e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54074943"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Políticas de Retenção no Exchange de Administração

Se quiser que executemos verificações automáticas das definições mencionadas abaixo, selecione o botão Back < -- na parte superior desta página e, em seguida, introduza o endereço de e-mail do utilizador que tem problemas com as políticas de retenção.

Se tiver problemas com as políticas de retenção no Centro de Administração do Exchange não se aplicam a caixas de correio ou itens que não estão a ser movidos para a caixa de correio de arquivo, verifique o seguinte:

**Causas Raiz:**

- **O Assistente de Pastas** Geridas não processou a caixa de correio do utilizador. O Assistente de Pastas Geridas tenta processar todas as caixas de correio na sua organização baseada na nuvem uma vez a cada sete dias.

  **Solução:** Execute o Assistente de Pastas Geridas.

- **O RetentionHold** foi **ativado** na caixa de correio. Se a caixa de correio tiver sido colocada num RetentionHold, a política de retenção na caixa de correio não será processada durante esse período de tempo.

  **Solução:** Verifique o estado da definição e atualização da Retenção conforme necessário. Para obter detalhes, consulte [o artigo Retenção na Caixa de Correio](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
 
**Nota:** Se uma caixa de correio for inferior a 10 MB, o Assistente de Pastas Geridas não processará automaticamente a caixa de correio.
 
Para mais informações sobre políticas de retenção no centro Exchange administração, consulte:

- [Etiquetas de retenção e políticas de retenção](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- [Aplicar uma política de retenção a caixas de correio](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) ou [Adicionar ou remover etiquetas de retenção](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)

- [Como identificar o tipo de reter colocado numa caixa de correio](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
