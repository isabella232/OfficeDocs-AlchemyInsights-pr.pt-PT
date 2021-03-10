---
title: Utilize as linhas de segurança Microsoft Intune para configurar dispositivos Windows 10
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: b95454ec8ce8d0d69d1f55f7ce4adc596929e2de
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/10/2021
ms.locfileid: "50696378"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a>Utilize as linhas de segurança Microsoft Intune para configurar dispositivos Windows 10

As linhas de segurança intune ajudam a proteger os utilizadores e dispositivos. As linhas de base de segurança são os grupos pré-configurados das definições do Windows utilizados para aplicar um grupo conhecido de definições e valores predefinidos recomendados pelas equipas de segurança relevantes. Ao criar um perfil de base de segurança no Intune, cria-se um modelo que consiste em múltiplos perfis de configuração do dispositivo.

Quando implementa linhas de segurança para grupos de utilizadores ou dispositivos, as definições são aplicadas em dispositivos que funcionam nas versões windows 10 ou posteriores. Por exemplo, a linha de base de segurança de gestão de dispositivos móveis da Microsoft (MDM) ativa automaticamente (1) o BitLocker para unidades amovíveis, (2) requer a palavra-passe para desbloquear um dispositivo e (3) desativa a autenticação básica. Quando um valor predefinido não funciona para o seu ambiente, pode personalizar a linha de base para aplicar as definições de que necessita.

As linhas de base de segurança também ajudam a estabelecer um fluxo de trabalho seguro de ponta a ponta na Microsoft 365. Seguem-se alguns benefícios desta funcionalidade:
- Uma linha de base de segurança inclui as melhores práticas e recomendações para configurações que afetam a segurança. Uma vez que a Intune é parceira da equipa de segurança do Windows que cria linhas de base para políticas de grupo, estas recomendações baseiam-se numa orientação sólida e numa vasta experiência.
- Se é novo no Intune e não sabe por onde começar, então as linhas de segurança irão ajudá-lo a criar rapidamente e a implementar um perfil seguro.
- Se está a usar uma política de grupo, então migrar para Intune para fins de gestão é muito mais fácil com bases de segurança, porque estas linhas de base de segurança são incorporadas no Intune e incluem capacidades de ponta para a gestão.

Para obter mais informações, consulte [as linhas de base de segurança do Windows](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) e a [gestão de dispositivos Móveis.](https://docs.microsoft.com/windows/client-management/mdm/)