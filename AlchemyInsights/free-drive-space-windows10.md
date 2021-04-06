---
title: Libertar espaço em disco no Windows 10
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9774"
- "9005390"
- "9005403"
ms.openlocfilehash: 2313636307bfddce2810c2d4c4ce9e3b407a7bdf
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505367"
---
# <a name="free-up-drive-space-in-windows-10"></a>Libertar espaço em disco no Windows 10

Eis duas opções para libertar espaço em disco no Windows:

- Liberte espaço em disco no Windows 10.
- Liberte espaço para as atualizações do Windows 10 com dispositivos de armazenamento externo.

Se ainda tiver pouco espaço em disco após utilizar a Limpeza do Disco, é possível que a sua pasta Temporária esteja a ficar rapidamente cheia de ficheiros de aplicação (.appx) utilizados pela Microsoft Store. Para corrigir este problema, reponha a Store, limpe a cache da Store e, em seguida, execute a resolução de problemas do Windows Update. Certifique-se de que a Microsoft Store está fechada antes de seguir estes passos.

**Passo 1: repor a Microsoft Store**

**Nota** Esta ação elimina permanentemente os dados da aplicação no dispositivo, incluindo as suas preferências e detalhes de início de sessão.

1. Selecione **Iniciar** > **Definições** > **Aplicações** > **Aplicações e funcionalidades**.

1. Na lista de aplicações, localize e selecione Microsoft Store.

1. Selecione **Opções avançadas**.

1. Desloque-se para baixo e selecione **Repor** e, em seguida, **Confirmar Reposição**.

**Passo 2: limpar a cache da Microsoft Store**

1. Prima a tecla do logótipo do Windows + R para abrir a caixa de diálogo Executar.

1. Escreva wsreset.exe e selecione **OK**.

1. É aberta uma janela de Linha de Comandos em branco. Após cerca de 10 segundos, a janela é fechada e a Store é aberta automaticamente.

**Passo 3: repor o Windows Update**

1. Selecione **Iniciar** > **Definições** > **Atualizar e Segurança** > **Resolução de Problemas**.

1. Desloque-se para baixo e selecione **Windows Update** a partir da lista e, em seguida, **Executar a resolução de problemas**.

1. Reinicie o computador e verifique se o problema ainda está presente.

