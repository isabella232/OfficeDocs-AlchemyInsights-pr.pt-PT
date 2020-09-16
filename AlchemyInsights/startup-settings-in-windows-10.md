---
title: Definições de arranque no Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001691"
- "3768"
ms.openlocfilehash: e49faca66785c6611dda702a381c39cdb10884f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751146"
---
# <a name="startup-settings-in-windows-10"></a>Definições de arranque no Windows 10

**Alterar quais aplicações são executadas automaticamente no arranque**

1. Vá a [Definições > Apps > Startup](ms-settings:startupapps?activationSource=GetHelp).

2. Certifique-se de que qualquer aplicação que pretenda executar no arranque está **ligada**.

**Adicione uma app para executar automaticamente no arranque**

1. Clique ou toque **em Iniciar** e encontre a aplicação que pretende executar no arranque.

2. Clique com o botão direito na aplicação, clique em **Mais**e, em seguida, clique em **Abrir a localização do ficheiro**. Isto abre o local onde o atalho para a aplicação é guardado. Se não houver opção para a localização do ficheiro Aberto, significa que a aplicação não pode ser executada no arranque.

3. Com a localização do ficheiro aberta, prima a **tecla**do logótipo do Windows + R , tipo **shell:startup,** em seguida, clique em **OK**. Isto abre a pasta Startup.

4. Copie e cole o atalho para a aplicação desde a localização do ficheiro até à pasta Startup.

**Opções avançadas de arranque (incluindo modo de segurança, definições UEFI e arranque de outro dispositivo)**

1. Guarde o seu trabalho e feche quaisquer documentos abertos, uma vez que estes passos reiniciarão o seu PC.

2. Ir para [Definições > Atualizar & recuperação > de segurança](ms-settings:recovery?activationSource=GetHelp).

3. No **arranque avançado,** clique **em Reiniciar agora**. 

4. Depois do seu PC reiniciar para o ecrã de opção Escolha:

    - Para arrancar a partir de um dispositivo como uma unidade USB, clique em **Utilizar um dispositivo**.

    - Para introduzir as definições UEFI (por vezes chamada configuração BIOS), clique em **Resolução de Problemas > Opções Avançadas > Definições de Firmware UEFI**. 

    - Para introduzir o Modo de Segurança ou alterar as definições avançadas de arranque, clique em **Troubleshoot > Opções Avançadas > Configurações de Arranque**, clique em **"Reiniciar"** Pode ser-lhe pedido que introduza a sua [chave de recuperação BitLocker](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key). Depois de o seu PC recomeçar, clique na definição de arranque que pretende utilizar.