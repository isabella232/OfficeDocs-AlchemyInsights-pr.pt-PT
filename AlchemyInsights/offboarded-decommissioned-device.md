---
title: Problemas com a remoção de um dispositivo offboarded ou desmissionado do Inventário de Dispositivos
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002913"
- "11187"
ms.openlocfilehash: 13865acb75b60a824c1dde9427c11471e980ea9e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324455"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a>Problemas com a remoção de um dispositivo offboarded ou desmissionado do Inventário de Dispositivos

O Microsoft Defender para Pontos Finais não permite atualmente a remoção manual do registo do dispositivo de um dispositivo offboarded ou desmissionado do Inventário de Dispositivos.

Por questões de segurança, o dispositivo permanece no portal como um registo histórico durante até 180 dias. No entanto, os dados do dispositivo são retidos de acordo com o período de retenção configurado.

**Nota:** Um dispositivo offboarded ou desativado muda automaticamente para o estado **Inativo** após sete dias. Além disso, os dispositivos que não estão ativos nos últimos 30 dias não serão faturados nos dados que refletem a pontuação de exposição Gestão de Vulnerabilidades e Ameaças organização ou a Pontuação Segura da Microsoft para Dispositivos.
 
Se ainda não quiser ver determinados dispositivos na vista Inventário de Dispositivos, experimente colocar uma etiqueta de dispositivo para filtrar o dispositivo des descomplicado a partir da vista Inventário de Dispositivos.

Para mais informações, consulte:

[Dispositivos offboard do serviço Microsoft Defender para Endpoint](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/offboard-machines.md)

[Pontuação de exposição Gestão de Vulnerabilidades e Ameaças](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[Corrigir sensores desalojáveis no Microsoft Defender para Endpoint](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[Como utilizar a etiquetação de forma eficaz (Parte 1)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[Como utilizar a etiquetação de forma eficaz (Parte 2)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[Como utilizar a etiquetação de forma eficaz (Parte 3)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




