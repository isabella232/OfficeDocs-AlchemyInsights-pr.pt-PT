---
title: Mover mensagens de e-mail para a caixa de correio arquivo
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
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 7e72766f441e210a81fcfd6c07b1801f6c0474afb02a70edf2ad8dbb571f3d2a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53974968"
---
# <a name="move-email-to-the-archive-mailbox"></a>Mover e-mails para a caixa de correio de arquivo

Se quiser que executemos verificações automáticas das definições mencionadas abaixo, selecione o botão Voltar <-- na parte superior desta página e, em seguida, introduza o endereço de e-mail do utilizador que tem problemas em mover e-mails para a respetiva caixa de correio de arquivo.

1. Confirme que **uma caixa de correio de Arquivo** foi ativada. Caso não o seja, utilize os passos [neste artigo para](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) ativar a caixa de correio de arquivo.

2. Para arquivar mensagens automaticamente na caixa de correio de  arquivo, uma etiqueta de retenção com a ação Mover para o arquivo tem de ser definida para ser aplicada automaticamente a toda a caixa de correio **(predefinição).** Utilize os passos aqui para criar a etiqueta: [Arquivar etiqueta predefinida](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Em seguida, adicione **a etiqueta Arquivo** à sua política de retenção. No centro de Exchange de Administração, selecionar Políticas de **Retenção** > adicione a etiqueta Mover para **o** Arquivo à política > **Guardar.**

4. Atribuir [a Política de Retenção à](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) caixa de correio do utilizador específico. A mesma política será aplicada à caixa de **correio** Principal e **ao** Arquivo.

Poderá ser necessário forçar o Assistente de Pastas Geridas (MFA) a executar e aplicar as novas definições à caixa de correio do utilizador. Execute o seguinte comando enquanto [estiver ligado ao EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) para iniciar o Assistente de Pastas Geridas de uma caixa de correio específica:
  
Start-ManagedFolderAssistant -Identity <name of the mailbox>

Para obter mais informações sobre como configurar uma política de arquivo, consulte Configurar uma política de arquivo e [eliminação para caixas de correio.](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)
  