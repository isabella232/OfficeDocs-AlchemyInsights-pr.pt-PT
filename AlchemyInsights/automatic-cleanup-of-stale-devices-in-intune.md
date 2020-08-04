---
title: Limpeza automática de dispositivos em intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 874ee290c59df3b5de1421369484a1a5a0ff7be4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555227"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a>Limpeza automática de dispositivos em intune

O Intune permite que o administrador configuure um intervalo de tempo entre 90 e 270 dias, após o qual os dispositivos em contrao tempo são removidos do serviço. Esta definição é ampla e uma vez ativada entra em vigor imediatamente. Quaisquer dispositivos não verificados no servidor Intune durante um período que exceda a definição são permanentemente eliminados.

**Nota** Apenas os objetos do dispositivo MDM são elegíveis para esta ação de limpeza. Excluem-se apenas objetos de dispositivoS EAS.

Para informações adicionais sobre quando um dispositivo se torna elegível para eliminação com base na configuração de limpeza do dispositivo e no seu "estado":

Definição: **Eliminar dispositivos após a última data de check-in: Sim (algum valor (N) em dias especificados)**

- Com base no valor (N) configurado na definição, o serviço Intune elimina o dispositivo nos dias especificados após a última verificação com sucesso.

Definição: **Eliminar dispositivos após a última data de check-in: Não**

- 180 dias após o termo do certificado do dispositivo e não ser renovado, o dispositivo é eliminado.

**Nota** Em ambos os casos, o dispositivo deve ser registado com sucesso no Intune. O registo ocorre durante o primeiro check-in do dispositivo com o serviço Intune.

Se um dispositivo se inscrever com sucesso no Intune mas não se tornar intune registado, o dispositivo é eliminado 270 dias após a inscrição. (90 dias para marcar o dispositivo como revogado e, em seguida, mais 180 dias para apagar o registo.)

Não existe atualmente nenhum mecanismo na consola Intune para estabelecer a data de validade da certificação do dispositivo para qualquer dispositivo.