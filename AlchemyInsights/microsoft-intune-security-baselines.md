---
title: Utilizar Microsoft Intune de base de segurança para configurar Windows 10 dispositivos
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: 88525fccd6dcde0cb3949e348d1f2a7df3ee7ce7
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793893"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Utilizar Microsoft Intune de base de segurança para configurar Windows 10 dispositivos

As linhas de base de segurança do Intune ajudam a proteger os utilizadores e os dispositivos. As linhas de base de Windows são grupos pré-configurados e configurados para aplicar um grupo conhecido de definições e valores predefinidos recomendados pelas equipas de segurança relevantes. Ao criar um perfil de linha de base de segurança no Intune, cria um modelo que consiste em múltiplos perfis de configuração de dispositivos.

Ao implementar linhas de base de segurança em grupos de utilizadores ou dispositivos, as definições são aplicadas a dispositivos que são executados Windows 10 ou posterior. Por exemplo, a linha de base de segurança da gestão de dispositivos móveis (MDM) da Microsoft ativa automaticamente o BitLocker em unidades amovíveis, requer a palavra-passe para desbloquear um dispositivo e desativa a autenticação básica. Quando um valor predefinido não funcionar no seu ambiente, pode personalizar a linha base para aplicar as definições de que precisa.

As linhas de base de segurança também ajudam a estabelecer um fluxo de trabalho seguro ponto a ponto no Microsoft 365. Uma linha base de segurança inclui as práticas recomendadas e recomendações para definições que afetam a segurança. O Intune tem parcerias com Windows equipa de segurança do Intune que cria linhas de base para políticas de grupo, pelo que estas recomendações baseiam-se em orientações sólidas e numa experiência extensa.

Se é novo no Intune e não sabe por onde começar, as linhas de base de segurança ajudam-no a criar e a implementar rapidamente um perfil seguro. Se utiliza atualmente uma política de grupo, é muito mais fácil migrar para o Intune para fins de gestão com linhas de base de segurança, uma vez que estão incorporadas no Intune e incluem funcionalidades de gestão de margem superior.

Para saber mais, consulte o Windows [de base de segurança e a gestão](/windows/security/threat-protection/windows-security-baselines) de [dispositivos móveis.](/windows/client-management/mdm/)

