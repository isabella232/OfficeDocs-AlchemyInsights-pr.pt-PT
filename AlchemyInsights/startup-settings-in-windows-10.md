---
title: Definições de arranque no Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001691"
- "3768"
ms.openlocfilehash: 526b92013f26675b5bf42077271ae7dc7003af31fa8f605d76aea92e0ccabfa1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53909837"
---
# <a name="startup-settings-in-windows-10"></a>Definições de arranque no Windows 10

**Alterar as aplicações executáveis automaticamente no arranque**

1. Vá para [o Definições > aplicações > Arranque.](ms-settings:startupapps?activationSource=GetHelp)

2. Certifique-se de que qualquer aplicação que pretende executar no arranque está **ativo**.

**Adicionar uma aplicação para ser executada automaticamente no arranque**

1. Clique ou toque **em Iniciar** e encontre a aplicação que pretende executar no arranque.

2. Clique com o botão direito do rato na aplicação, clique **em Mais e,** em seguida, clique **em Abrir localização do ficheiro**. Esta ação abre a localização onde o atalho da aplicação é guardado. Se não houver nenhuma opção para Abrir localização do ficheiro, significa que a aplicação não pode ser executada no arranque.

3. Com a localização do ficheiro aberta, prima a tecla do logótipo **do Windows + R,** escreva **shell:startup** e, em seguida, clique em **OK.** Esta ação abre a pasta Arranque.

4. Copie e copie o atalho para a aplicação a partir da localização do ficheiro para a pasta Arranque.

**Opções de arranque avançadas (incluindo o Modo Cofre Desinserção, as definições UEFI e o arranque a partir de outro dispositivo)**

1. Guarde o seu trabalho e feche todos os documentos abertos, uma vez que estes passos irão reiniciar o seu PC.

2. Vá para [Atualizar Definições > atualização & segurança > Recuperação.](ms-settings:recovery?activationSource=GetHelp)

3. Em **Arranque avançado, clique** em **Reiniciar agora**. 

4. Depois de o PC reiniciar para o ecrã Selecionar uma opção:

    - Para ser iniciado a partir de um dispositivo como uma pen USB, clique **em Utilizar um dispositivo**.

    - Para introduzir as definições UEFI (por vezes denominadas configuração BIOS), clique em > Opções avançadas > **firmware UEFI Definições**. 

    - Para entrar no modo Cofre de arranque ou alterar as definições de arranque avançadas, clique em Resolução de > Opções **avançadas >** de Arranque Definições e, em seguida, clique **em Reiniciar**. Poderá ser-lhe pedido que introduza a [sua chave de recuperação BitLocker.](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key) Após o PC reiniciar, clique na definição de arranque que pretende utilizar.