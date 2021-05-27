---
title: Estado do sensor de verificação do Ponto Final do Defender
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: a53a0109c3b974806d04135dd2c102de81ec560f
ms.sourcegitcommit: ded29f44e5019b1929218b02733b390899843680
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/24/2021
ms.locfileid: "52676340"
---
# <a name="defender-endpoint-check-sensor-status"></a>Estado do sensor de verificação do Ponto Final do Defender

O **mosaico Dispositivos com** problemas de sensor encontra-se no dashboard Operações de Segurança. Este mtilo fornece informações sobre a capacidade de um dispositivo individual fornecer dados de sensor e comunicar com o serviço Defender para Pontos Finais. Reporta quantos dispositivos necessitam de atenção e ajuda-o a identificar dispositivos problemáticos e a tomar medidas para corrigir problemas conhecidos.

Dois indicadores de estado no mosaico fornecem informações sobre o número de dispositivos que não comunicam corretamente ao serviço:

- **Configurado inde forma erradamente** Os dispositivos que podem estar parcialmente a comunicar dados do sensor ao Defender para serviço de Pontos Finais e podem ter erros de configuração que precisam de ser corrigidos.
- **Inativo** Dispositivos que deixaram de comunicar com o Defender para serviço de Pontos Finais durante mais de sete dias no último mês.

Ao clicar em qualquer um dos grupos, é direcionado para a lista Dispositivos, filtrado de acordo com as suas opções. Na lista de Dispositivos, pode filtrar a lista do estado de saúde pelo seguinte estado:

- **Ativo** Dispositivos que comunicam ativamente ao serviço do Defender para Pontos Finais.
- **Configurado inde forma erradamente** Os dispositivos que podem estar parcialmente a comunicar dados do sensor ao Defender para serviço de Pontos Finais, mas que têm erros de configuração que têm de ser corrigidos. Os dispositivos mal configurados podem ter um ou uma combinação dos seguintes problemas:

    - Sem dados do sensor – os dispositivos deixaram de enviar dados do sensor. Os alertas limitados podem ser ativados a partir do dispositivo.
    - Comunicações com deficiências - a capacidade de comunicar com dispositivos é prejudicada. Enviar ficheiros para uma análise aprofundada, bloquear ficheiros, isolar o dispositivo da rede e outras ações que exijam comunicação com o dispositivo poderá não funcionar.
- **Inativo** Dispositivos que deixaram de comunicar com o Serviço de Pontos Finais do Defender.

Pode transferir a lista completa no formato CSV com a funcionalidade Exportar.

Para obter mais informações, consulte [Verificar o estado de funcionamento do sensor no Microsoft Defender para Endpoint.](/microsoft-365/security/defender-endpoint/check-sensor-status)

Para obter mais informações sobre o que fez com que um dispositivo se encontrasse inativo ou mal configurado, consulte Corrigir sensores não em mau estado de funcionamento no [Microsoft Defender para o Endpoint.](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors)
