---
title: Configurações de arranque no Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001691"
- "3768"
ms.openlocfilehash: b4854944d8cbd9bd83fdea609007c15d39c8eb75
ms.sourcegitcommit: c55eea624d960d2dd17ac4aa5a4c23e34e6443b8
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/04/2020
ms.locfileid: "42409234"
---
# <a name="startup-settings-in-windows-10"></a>Configurações de arranque no Windows 10

**Alterar quais as aplicações que funcionam automaticamente no arranque**

1. Vá a [Definições > Apps > Startup](ms-settings:startupapps?activationSource=GetHelp).

2. Certifique-se de que qualquer aplicação que pretenda executar no arranque está **ligada**.

**Adicione uma aplicação para executar automaticamente no arranque**

1. Clique ou toque **em Iniciar** e encontre a app que pretende executar no arranque.

2. Clique na aplicação, clique em **Mais,** e clique na localização do **ficheiro Open**. Isto abre o local onde o atalho para a aplicação é guardado. Se não houver opção para a localização do ficheiro Open, significa que a aplicação não pode funcionar no arranque.

3. Com a localização do ficheiro aberta, prima a **tecla do logótipo do Windows + R,** tipo **shell:startup,** e, em seguida, clique EM **OK**. Isto abre a pasta Startup.

4. Copie e cole o atalho na aplicação desde a localização do ficheiro até à pasta Startup.

**Opções avançadas de arranque (incluindo Modo Seguro, definições UEFI e arranque de outro dispositivo)**

1. Guarde o seu trabalho e feche quaisquer documentos abertos, uma vez que estes passos irão reiniciar o seu PC.

2. Vá a [Definições > Atualizar & Recuperação](ms-settings:recovery?activationSource=GetHelp)de > de Segurança .

3. Em **arranque avançado,** clique **em Reiniciar agora**. 

4. Depois de o pc reiniciar para o ecrã Escolha um ecrã de opção:

    - Para arrancar de um dispositivo como uma unidade USB, clique **em Utilizar um dispositivo**.

    - Para introduzir as definições UEFI (por vezes chamada de configuração BIOS), clique em **Troubleshoot > Opções avançadas > Definições de Firmware UEFI**. 

    - Para introduzir o Modo Seguro ou alterar as definições avançadas de arranque, clique em **Resolução de problemas > opções avançadas > Definições**de Arranque e, em seguida, clique em **Reiniciar**. Pode ser-lhe pedido que introduza a [sua chave de recuperação BitLocker](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key). Depois de o seu PC recomeçar, clique na definição de arranque que pretende utilizar.