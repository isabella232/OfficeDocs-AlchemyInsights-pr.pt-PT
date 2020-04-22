---
title: Mover mensagens de correio eletrónico para a caixa de correio do Arquivo
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: a5ad81e97df0ed5c337a622126173df94af80bb8
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713657"
---
# <a name="move-email-to-the-archive-mailbox"></a>Mova o e-mail para a caixa de correio de arquivo

1. Confirme que foi ativada uma **caixa de correio Archive.** Caso contrário, utilize os passos [deste artigo](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) para ativar a caixa de correio de arquivo.

2. Para arquivar mensagens automaticamente na caixa de correio de arquivo, deve ser definida uma etiqueta de retenção com o **Movimento para arquivar** ação para ser aplicada automaticamente à etiqueta inteira da caixa de correio **(predefinido).** Utilize os passos aqui para criar a etiqueta: [Etiqueta padrão de arquivo](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Em seguida, adicione a etiqueta **de Arquivo** à sua política de retenção. No centro de administração exchange, escolha Políticas de **Retenção** > adicione a **etiqueta Move to Archive** à política > **Save**.

4. Agora [atribua a Política](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) de Retenção à caixa de correio do utilizador específico. A mesma política será aplicada tanto à **Primary** como à **Caixa** de Correio seleções.

Pode ser necessário forçar o Assistente de Pasta Gerida (MFA) a executar e aplicar as novas definições na caixa de correio do utilizador. Executar o seguinte comando enquanto [ligado ao EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) para iniciar o Assistente de Pasta Gerida para uma caixa de correio específica:
  
Assistente de Pasta Gerido por Início -Identidade<name of the mailbox>

Para obter mais informações sobre a criação de uma política de arquivo, consulte [A criação de uma política de arquivo e eliminação para caixas de correio](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  