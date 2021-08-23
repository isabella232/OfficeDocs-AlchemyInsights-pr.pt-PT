---
title: Alertas em falta no separador Alertas
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9007647"
- "12732"
ms.openlocfilehash: 9fbd9a32e40d858f0ba49931c723a824478aaa12
ms.sourcegitcommit: 2be4a0352cb84a703ebf12966e1c17b64df07364
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/16/2021
ms.locfileid: "58454970"
---
# <a name="alerts-missing-from-alerts-tab"></a>Alertas em falta no separador Alertas

O **separador Alertas** funciona com base na configuração e nas políticas ativadas a partir do portal Governação de Aplicações no seu inquilino. As políticas externas à migração de aplicações também têm de ser ativadas para permitir que os sinais sejam apresentados no **separador Alertas.** 

Confirme que o alerta foi gerado:

1. Vá para Políticas de governação [da aplicação](https://compliance.microsoft.com/m365appprotection?viewid=policies) e confirme se criou, pelo menos, uma política Ativa ou de auditoria.

1. Selecione a política e, em seguida, **selecione Editar** no painel de panfleto. 

1. Verifique a configuração da política para confirmar que um alerta deve ter sido gerado com base num evento de política iniciado há mais de 24 horas.

Para obter mais informações sobre alertas na Gestão de Aplicações, consulte Começar a deteção e remediação de ameaças [de aplicações.](https://docs.microsoft.com/microsoft-365/compliance/app-governance-detect-remediate-get-started)