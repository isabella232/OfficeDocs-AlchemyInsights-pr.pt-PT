---
title: Utilizar Microsoft Intune de base de segurança para configurar Windows 10 dispositivos
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
ms.openlocfilehash: a94c6b72df3874ee80413adac86d60306175734b6ff28b2e015e05eec6f3838b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104355"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Utilizar Microsoft Intune de base de segurança para configurar Windows 10 dispositivos

As linhas de base de segurança do Intune ajudam a proteger os utilizadores e os dispositivos. As linhas de base de Windows são grupos pré-configurados das definições utilizados para aplicar um grupo conhecido de definições e valores predefinidos recomendados pelas equipas de segurança relevantes. Ao criar um perfil de linha de base de segurança no Intune, cria um modelo que consiste em múltiplos perfis de configuração de dispositivos.

Ao implementar linhas de base de segurança em grupos de utilizadores ou dispositivos, as definições são aplicadas a dispositivos que são executados Windows 10 ou posterior. Por exemplo, a Linha de Base de Segurança MDM ativa automaticamente (1) o BitLocker para unidade amovível (2) requer a palavra-passe para desbloquear um dispositivo e (3) desativa a autenticação básica. Quando um valor predefinido não funcionar no seu ambiente, personalize a linha de base para aplicar as definições de que precisa.

As linhas de base de segurança também ajudam a estabelecer um fluxo de trabalho seguro ponto a ponto no Microsoft 365. Seguem-se algumas vantagens desta situação:

- Uma linha base de segurança inclui as práticas recomendadas e recomendações para definições que afetam a segurança. Uma vez que o Intune tem parcerias com Windows equipa de segurança do Windows que cria linhas de base para políticas de grupo, estas recomendações baseiam-se em orientações sólidas e numa experiência extensa.
- Se não estiver novo no Intune e não tiver a certeza de onde deve começar, as linhas de base de segurança irão ajudá-lo a criar e a implementar rapidamente um perfil seguro.
- Se utiliza atualmente uma política de grupo, é muito mais fácil migrar para o Intune para fins de gestão com linhas de base de segurança, uma vez que estão incorporadas no Intune e incluem funcionalidades de primeira utilização para gestão.

Para saber mais, consulte o Windows [de base de segurança e a gestão](https://go.microsoft.com/fwlink/?linkid=2141503) de [dispositivos móveis.](https://go.microsoft.com/fwlink/?linkid=2141701)