---
title: Mitigar o erro A aplicação não foi detetada
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000171"
- "1712"
ms.openlocfilehash: 34b2024257c88512db170cbb0e672c1628ad8e3935342f87c5032492e1ad0259
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54026125"
---
# <a name="mitigate-the-application-was-not-detected-error"></a>Mitigar o erro "A aplicação não foi detetada"

O erro de instalação da aplicação, "A aplicação não foi detetada após a instalação ter sido concluída com êxito", reportado pelo Intune, pode ocorrer em todas as principais plataformas de SO (Windows, iOS e Android).

Os cenários mais comuns que geram este erro incluem:

- A aplicação foi atualizada fora de Intune (a partir de uma loja de aplicações de terceiros) após a implementação inicial. Por exemplo, algumas aplicações como o Google Chrome podem realizar atualizações automáticas.
- Um utilizador desinstalou a aplicação após a instalação inicial.

Para mitigar este problema, reveja primeiro os dispositivos afetados para determinar o cenário em que o erro ocorre.

- Se a aplicação tiver sido atualizada fora do Intune, a implementação da aplicação pode ser definida para ignorar a versão da aplicação. Para tal, em **Configuração da Aplicação > Informações da Aplicação**, defina **Ignorar a versão da aplicação** como **Sim**.
- Ao focar-se no cliente, poderá ser apropriado implementar a aplicação como "necessária", e garantir que a versão mais recente é implementada.
- Em alternativa, na plataforma iOS, é possível utilizar a funcionalidade de **atualização automática** associada ao Programa de Compra em Volume da Apple, que pode ser configurada para atualizar automaticamente para novas versões de aplicações à medida que forem disponibilizadas.

Para obter mais informações sobre resolução de problemas de instalação de aplicações, consulte [Resolver problemas de instalação de aplicações](https://docs.microsoft.com/intune/troubleshoot-app-install).
