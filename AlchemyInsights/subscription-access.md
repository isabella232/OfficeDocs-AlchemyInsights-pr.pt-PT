---
title: Acesso à subscrição
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
- "9003799"
- "6805"
ms.openlocfilehash: 166380cff09f2a2bd9b7e8914d5db4071b6c3f12
ms.sourcegitcommit: bec3554bf061ef28a009f460fb9d0a661b4fc008
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807718"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>Não é possível iniciar súmia devido a problemas de navegador (Browser hangs, continua a girar, não carrega, etc.)

Pode ser afetado por uma paragem. Por favor, verifique se há uma paragem em curso: [Azure Health Status](https://status.azure.com/status/history/).

Por favor, faça login em todas as sessões ativas do Azure. Inicie um modo inuginal ou incógnito do seu navegador web.

Também pode tentar refrescar o navegador, usar outro navegador, eliminar cookies de cache se acima não funcionar.

Saiba mais: [Problemas de resolução de problemas](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**Não conseguir aceder a subscrições**

No [portal Azure,](https://portal.azure.com/)certifique-se de que o diretório Azure correto é selecionado a partir da conta no topo direito.

No [centro de Conta Azure,](https://account.windowsazure.com/Subscriptions)certifique-se de que a conta utilizada é a administração da conta.

Saiba mais: [Resolução de problemas Sem Subscrições encontradas](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**Incapaz de aceder ao histórico de faturação**

O administrador da conta tem de se certificar de que o utilizador que acede às informações de faturação é adicionado no diretório Azure Ative como utilizador convidado: [Adicionar ou eliminar um novo utilizador](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

O utilizador tem então de ter um papel de administrador global: [Atribuir função aos utilizadores](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Publique isto, o utilizador pode ter acesso à faturação utilizando as políticas do RBAC: [Conceder acesso à faturação](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).

**Documentos Recomendados**

-   [Não posso entrar para gerir a minha assinatura do Azure.](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)