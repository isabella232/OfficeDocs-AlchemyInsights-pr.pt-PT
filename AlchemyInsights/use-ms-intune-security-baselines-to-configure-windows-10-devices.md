---
title: Utilize linhas de segurança Microsoft Intune para configurar dispositivos Windows 10
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: 24257f1ac5752df1598d08fcfdb95ee2642adfea
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573534"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Utilize linhas de segurança Microsoft Intune para configurar dispositivos Windows 10

As linhas de segurança intune ajudam a proteger os utilizadores e dispositivos. As linhas de base de segurança são os grupos pré-configurados das definições do Windows utilizados para aplicar um grupo conhecido de definições e valores predefinidos recomendados pelas equipas de segurança relevantes. Ao criar um perfil de base de segurança no Intune, cria-se um modelo que consiste em múltiplos perfis de configuração do dispositivo.

Quando implementa linhas de segurança para grupos de utilizadores ou dispositivos, as definições são aplicadas em dispositivos que funcionam no Windows 10 ou posteriormente. Por exemplo, o MD Security Baseline automaticamente (1) permite que o BitLocker para unidades amovíveis, (2) requer a palavra-passe para desbloquear um dispositivo, e (3) desativa a autenticação básica. Quando um valor predefinido não funcionar para o seu ambiente, personalize a linha de base para aplicar as definições de que necessita.

As linhas de base de segurança também ajudam a estabelecer um fluxo de trabalho seguro de ponta a ponta na Microsoft 365. Seguem-se alguns benefícios:

- Uma linha de base de segurança inclui as melhores práticas e recomendações para configurações que afetam a segurança. Uma vez que a Intune é parceira da equipa de segurança do Windows que cria linhas de base para políticas de grupo, estas recomendações baseiam-se numa orientação sólida e numa vasta experiência.
- Se é novo no Intune e não sabe por onde começar, então as linhas de segurança irão ajudá-lo a criar rapidamente e a implementar um perfil seguro.
- Se você usa atualmente uma política de grupo, então migrar para Intune para fins de gestão é muito mais fácil com linhas de base de segurança, porque eles são incorporados no Intune e incluem capacidades de ponta para gestão.

Para saber mais, consulte [as linhas de base de segurança do Windows](https://go.microsoft.com/fwlink/?linkid=2141503) e a [gestão de dispositivos móveis.](https://go.microsoft.com/fwlink/?linkid=2141701)