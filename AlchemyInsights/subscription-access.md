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
ms.openlocfilehash: b138c05e87e70c18bb6528819a34f8a9501446d57dcf4dbac0734f70fbc3466b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53999251"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>Não é possível o Azure de inscrever-se devido a problemas do browser (o browser para, continua a girar, não carrega, etc.)

Poderá ser afetado por uma insucesse. Verifique se existe uma insuceção em curso: Estado de [Saúde do Azure](https://status.azure.com/status/history/).

Ter sessão em todas as sessões ativas do Azure. Inicia um modo privado ou incógnito do seu browser.

Também pode tentar Atualizar o browser, utilizar outro browser e eliminar cookies de cache se acima não funcionar.

Saiba mais: [Remoção de Problemas de Lote](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**Não é possível aceder a subscrições**

No portal do [Azure](https://portal.azure.com/), certifique-se de que o diretório do Azure correto está selecionado a partir da conta no canto superior direito.

No Centro [de Contas do Azure,](https://account.windowsazure.com/Subscriptions)certifique-se de que a conta utilizada é o administrador de conta.

Saiba mais: [Remoção de Problemas não encontrados em Subscrições](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**Não é possível aceder ao histórico de faturação**

O administrador de conta tem de se certificar de que o utilizador que acede às informações de faturação é adicionado no Azure Active Directory como utilizador convidado: Adicionar ou eliminar um [novo utilizador.](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support)

Em seguida, o utilizador tem de ter uma função de administrador Global: [Atribuir função aos utilizadores.](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support)

Publicar isto, o utilizador pode ter acesso à faturação através de políticas RBAC: Conceder acesso [à faturação.](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)

**Documentos recomendados**

-   [Não consigo inscrever-me para gerir a minha subscrição do Azure](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)