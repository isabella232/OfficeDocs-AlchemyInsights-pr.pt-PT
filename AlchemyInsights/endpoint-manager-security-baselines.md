---
title: Endpoint Manager - Linhas de base de segurança
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
- "10064"
- "9003771"
ms.openlocfilehash: 4c8e03a817751ba7dc1710aed5a3e19c6e79db33
ms.sourcegitcommit: ae556b6b26974392ca68a68426a2b40967ae0071
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/07/2021
ms.locfileid: "58923565"
---
# <a name="endpoint-manager---security-baselines"></a>Endpoint Manager - Linhas de base de segurança

As linhas de base de segurança são grupos pré-configurados de definições do Windows que o ajudam a aplicar as definições de segurança recomendadas pelas equipas de segurança relevantes. Estas linhas de base podem ser personalizadas para aplicar apenas as definições e os valores pretendidos. Para obter mais informações sobre as linhas de base de segurança, consulte [Utilizar linhas de base de segurança para configurar dispositivos Windows 10 no Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).

Apenas existem linhas de base para estes produtos:

- Definições de segurança do Windows MDM
- Segurança do Microsoft Defender para Ponto Final
- Microsoft Edge

Cada uma das linhas de base é atualizada periodicamente e lançada em versões incrementais. Cada versão adiciona e/ou remove as definições da versão anterior para garantir que a linha de base cumpre as orientações atuais. A consola de Linhas de base de segurança no Endpoint Security permite-lhe comparar versões diferentes ao tornar visíveis as alterações de versão para versão.

Para obter orientações sobre a forma mais eficiente de alterar a versão da linha de base que é implementada, consulte [Gerir perfis de segurança de linha de base no Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).

Após implementar uma linha de base de segurança, pode monitorizar o estado da implementação e rever as definições dispositivo a dispositivo.

Uma vez que as linhas de base de segurança contêm muitas definições, é importante rever as alterações de configuração e efetuar testes para garantir que todas as definições são adequadas para os seus dispositivos e necessidades empresariais.

**Nota:** os dados de relatórios das linhas de base podem demorar até 24 horas a serem apresentados após a implementação inicial para um dispositivo, e até 6 horas para atualizações futuras. 

A causa mais comum de uma definição de linha de base não ser aplicada prende-se com o facto de a mesma definição estar a ser utilizada num perfil diferente. Este cenário pode ser investigado num dispositivo específico, ao selecionar o mesmo a partir do nó do Estado do Dispositivo do perfil de Linha de Base de segurança. Para obter detalhes, consulte [Resolver conflitos de linhas de base de segurança](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).