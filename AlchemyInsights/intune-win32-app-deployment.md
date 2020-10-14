---
title: Implementação de aplicativo Intune Win32
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/06/2020
ms.locfileid: "48461876"
---
# <a name="intune-win32-app-deployment"></a>Implementação de aplicativo Intune Win32

O Microsoft Intune permite aplicações Win32, incluindo, mas não se limitando a MSI e . O EXE vai ser implantado nos dispositivos do Windows 10. O mecanismo de implantação utilizado requer a presença da Extensão de Gestão intune (IME) no dispositivo-alvo. O IME será instalado automaticamente como resultado de uma configuração de configuração ou implementação de aplicação win32 para um utilizador/dispositivo.

Há também um conjunto de pré-requisitos que devem ser cumpridos para implementar aplicações Win32 que incluem:

- Plataformas suportadas: Versão 1607 ou posterior do Windows 10 (versões Enterprise, Pro e Education).
- Arquitetura suportada: x86 e x64.
- Gestão de Dispositivos: AAD aderiu e matriculada automaticamente (incluindo domínio híbrido e política de grupo auto-inscrita).
- Formato pacote de aplicação: . **ficheiro intunewin**  preparado pela ferramenta de preparação de [conteúdo microsoft Win32](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).
- Limitações:
    - Tamanho máximo: 8GB.
    - Arquitetura não suportada: ARMs.

Reveja o doc "[Add, assign, and monitor a Win32 app in Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" para obter informações relacionadas com esses passos.

Os detalhes sobre a implementação de aplicações de resolução de problemas no Windows, incluindo aplicações Win32, podem ser revistos nos seguintes documentos

- [Problemas de instalação de aplicativos de resolução de problemas](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [Resolução de problemas Aplicativos Win32](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)