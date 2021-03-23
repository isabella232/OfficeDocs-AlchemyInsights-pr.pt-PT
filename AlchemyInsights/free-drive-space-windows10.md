---
title: Espaço de unidade gratuito no Windows 10
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
- "9005403"
ms.openlocfilehash: 3838f3db3bc5f54bcb1a2558484056f3194b76e1
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037945"
---
# <a name="free-up-drive-space-in-windows-10"></a>Espaço de unidade gratuito no Windows 10

Aqui estão duas opções para libertar o espaço de condução no Windows:

- Liberte espaço de unidade no Windows 10.
- Liberte espaço para atualizações do Windows 10 com dispositivo de armazenamento externo.

Se ainda tiver pouco espaço em disco depois de utilizar a Disk Cleanup, é possível que a sua pasta Temp esteja rapidamente a preencher com ficheiros de aplicação (.appx) utilizados pela Microsoft Store. Para corrigir este problema, reinicie a Loja, limpe a cache da Loja e, em seguida, execute o resolução de problemas do Windows Update. Certifique-se de que a Microsoft Store está fechada antes de prosseguir com estes passos.

**Passo 1: Redefinir a Microsoft Store**

**Nota** Isto elimina permanentemente os dados da aplicação no dispositivo, incluindo as suas preferências e detalhes de início de saúde.

1. Selecione   >  **Iniciar Definições**  >    >  **Aplicações Apps & funcionalidades**.

1. Na lista de aplicações, localize e selecione a Microsoft Store.

1. Selecione **opções avançadas**.

1. Desloque-se para baixo e **selecione Reset** e, em seguida, **confirme reset**.

**Passo 2: Limpar a cache da Microsoft Store**

1. Prima a tecla do logotipo do Windows + R para abrir a caixa de diálogo executar.

1. Digite wsreset.exe e selecione **OK**.

1. Abre-se uma janela de pedido de comando em branco. Após cerca de 10 segundos, a janela fecha-se e a Loja abre-se automaticamente.

**Passo 3: Redefinir atualização do Windows**

1. Selecione **Iniciar**  >    >  **Atualização de Definições &**  >  **resolução de problemas de** segurança .

1. Desloque-se para baixo e selecione o **Windows Update** da lista e selecione **Executar o resolução de problemas**.

1. Reinicie o seu computador e verifique se ainda está a passar pelo problema.

