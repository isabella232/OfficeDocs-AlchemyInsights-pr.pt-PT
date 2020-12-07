---
title: Suporte do Microsoft Edge para Microsoft Defender Application Guard
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004024"
- "7090"
ms.openlocfilehash: 65cbc867ea7d1c73ca2906f51f72aa3376f31b5d
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/04/2020
ms.locfileid: "49584014"
---
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a>Suporte do Microsoft Edge para Microsoft Defender Application Guard

Projetado para o Windows 10 e Microsoft Edge, o Application Guard utiliza uma abordagem de isolamento de hardware que permite ao utilizador navegar num site não fideducionado a partir de dentro de um recipiente isolado, ativado por Hiper-V, separado do sistema operativo anfitrião.

Um administrador da empresa define uma lista de sites fidedignos, recursos em nuvem e redes internas. Quando um utilizador visita um site que não está na lista, o Microsoft Edge abrirá o site no contentor. Isto significa que se o site se revelar malicioso, o PC anfitrião permanecerá protegido e o intruso não chegará aos dados da empresa.

A instalação de extensões no contentor é suportada a partir da versão 81 do Microsoft Edge, e pode ser controlada através de uma política. O endereço updateURL que é utilizado na política ExtensionInstallForcelist deve ser adicionado como um Recurso Neutro nas políticas de isolamento de rede utilizadas pela Guard de aplicação.

Para obter mais informações, consulte [o suporte do Microsoft Edge para o Microsoft Defender Application Guard](https://go.microsoft.com/fwlink/?linkid=2134229).
