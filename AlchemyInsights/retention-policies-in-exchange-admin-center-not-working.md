---
title: As Políticas de Retenção no Centro de Administração do Exchange não funcionam
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
ms.openlocfilehash: bb2ce7ce2405be575dfdb79d304fef690e863a4e
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952239"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Políticas de Retenção no Centro de Administração do Exchange

Se quiser que executemos verificações automáticas das definições mencionadas abaixo, selecione o botão Back < -- na parte superior desta página e, em seguida, introduza o endereço de e-mail do utilizador que tem problemas com as políticas de retenção.

Se tiver problemas com as políticas de retenção no Centro de Administração do Exchange que não se aplicam a caixas de correio ou itens que não estão a ser movidos para a caixa de correio de arquivo, verifique o seguinte:

**Causas Raiz:**

- **O Assistente de Pastas** Geridas não processou a caixa de correio do utilizador. O Assistente de Pastas Geridas tenta processar todas as caixas de correio na sua organização baseada na nuvem uma vez a cada sete dias.

  **Solução:** Execute o Assistente de Pastas Geridas.

- **O RetentionHold** foi **ativado** na caixa de correio. Se a caixa de correio tiver sido colocada num RetentionHold, a política de retenção na caixa de correio não será processada durante esse período de tempo.

  **Solução:** Verifique o estado da definição e atualização da Retenção conforme necessário. Para obter detalhes, consulte [o artigo Retenção na Caixa de Correio](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
 
**Nota:** Se uma caixa de correio for inferior a 10 MB, o Assistente de Pastas Geridas não processará automaticamente a caixa de correio.
 
Para mais informações sobre políticas de retenção no Centro de Administração do Exchange, consulte:

- [Etiquetas de retenção e políticas de retenção](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- [Aplicar uma política de retenção a caixas de correio](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) ou [Adicionar ou remover etiquetas de retenção](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)

- [Como identificar o tipo de reter colocado numa caixa de correio](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
