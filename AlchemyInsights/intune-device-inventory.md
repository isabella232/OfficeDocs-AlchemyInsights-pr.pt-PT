---
title: Inventário de Dispositivos do Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: 00ee4f1d7130c239272e28ee8e051a18e6e0baf13040d2a892866be5900adfaf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54014083"
---
# <a name="intune-device-inventory"></a>Inventário de Dispositivos do Intune

A patina de Dispositivos fornece ao administrador informações sobre os dispositivos sob gestão no Intune numa base por dispositivo. As informações apresentadas incluem: Hardware, Aplicações descobertas, estado de Conformidade do Dispositivo e Estado de Configuração do Dispositivo.

Os dados de inventário para hardware e aplicações descobertas são recolhidos num ciclo de sete dias. As aplicações e os elementos específicos do hardware reportados diferem consoante o sistema operativo do dispositivo e se é pessoalmente ou propriedade da empresa.

Para obter mais informações, consulte [Ver detalhes do dispositivo no Intune.](https://docs.microsoft.com/intune/device-inventory)

**FAQ**

P: Não estou a receber uma lista de inventário completa das aplicações presentes nos dispositivos Windows Intune. Por que não?

R: Neste momento, só são listadas aplicações modernas para PCs Windows 10 identificados como dispositivos empresariais. O Intune não recolhe informações sobre as aplicações Win32 instaladas nestes dispositivos.

P: Por que motivo os números de telefone não são recolhidos de todos os dispositivos?

A: Os telefones categorizados como dispositivos empresariais no Intune não são identificados com o respetivo número de telefone completo quando, por exemplo, executa um relatório de inventário de dispositivos móveis. Os números de telefone com o seu próprio dispositivo estão sempre parcialmente mascarados com asteriscos (****) e só mostram os últimos quatro dígitos.