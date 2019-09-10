---
title: Mover mensagens de email para a caixa de correio arquivar
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 5592bc7d4566e3498c33bbf9488db7f46ec58842
ms.sourcegitcommit: 8864b5789d9905916039081b53530c7e6d8bc529
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822173"
---
# <a name="move-email-to-the-archive-mailbox"></a>Mover email para a caixa de correio de arquivamento

1. Confirme se uma **caixa de correio de arquivamento** foi habilitada. Caso não esteja, use as etapas neste [artigo](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) para habilitar a caixa de correio de arquivamento.

2. Para arquivar mensagens automaticamente na caixa de correio de arquivamento, uma marca de retenção com a ação **mover para arquivar** deve ser definida como **aplicada automaticamente à marca de caixa de correio inteira (padrão)**. Use as etapas aqui para criar a marca: [Archive default tag](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Em seguida, adicione a tag **Archive** à sua política de retenção. No centro de administração do Exchange, escolha **diretivas de retenção** > adicione a **tag mover para arquivar** na política > **salvar**.

4. Agora [atribua a política de retenção](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) à caixa de correio do usuário específico. A mesma política será aplicada ao **primário** e à caixa de correio de **arquivamento** .

Pode ser necessário forçar o assistente de pasta gerenciada (MFA) para executar e aplicar as novas configurações à caixa de correio do usuário. Execute o seguinte comando enquanto [estiver conectado ao EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) para iniciar o assistente de pasta gerenciada para uma caixa de correio específica:
  
Start-ManagedFolderAssistant-identidade<name of the mailbox>

Para obter mais informações sobre como configurar uma política de arquivamento, consulte [Configurar uma política de arquivamento e exclusão para caixas de correio](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  