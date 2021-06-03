---
title: A DLP do ponto final não está implementada no dispositivo do utilizador
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11470"
- "9000292"
ms.openlocfilehash: 948835f5468b480536c176bfdf3b4eefb76b3bdb
ms.sourcegitcommit: c32233a1b7e6f1b07913d25f90189a58a8de2560
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/27/2021
ms.locfileid: "52731864"
---
# <a name="endpoint-dlp-not-deployed-to-users-device"></a>A DLP do ponto final não está implementada no dispositivo do utilizador

Se a definição Prevenção de perda de dados do Ponto Final (DLP) não tiver sido aplicada ao dispositivo de um utilizador, confirme que cumpre estes requisitos:

- Windows 10 x64 com a complicação 1809 ou posterior instalada no dispositivo.
- É instalada a versão 4.18.2009.7 ou posterior do cliente anti-software.
- O dispositivo é **um** destes:
    
    - Azure Active Directory (Azure AD) associado
    - Aderido do Azure AD Híbrido
    - AAD registado

- Para impor ações de política, certifique-se de que o Microsoft Chromium browser Edge está instalado no dispositivo de ponto final.

Para obter requisitos adicionais para implementar o Endpoint DLP, consulte Começar a trabalhar com a prevenção de perda de dados [endpoint.](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints)