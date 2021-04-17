---
title: Monitorização existente da resolução de problemas
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: c4d2bb64b6b5ea79d4cd585e2be85c3c17e0f76f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824590"
---
# <a name="troubleshoot-an-existing-monitor"></a>Resolução de problemas de um monitor existente

Experimente estas soluções para resolver problemas num monitor. 

**Refresque o visor do monitor:**

Prima as seguintes teclas ao mesmo tempo: Tecla do Windows + Ctrl + Shift + B. Isto irá refrescar a comunicação com o seu controlador gráfico. Os seus monitores piscarão momentaneamente e voltarão após alguns segundos.

**Hardware do monitor de resolução de problemas:**

1. Desligue o cabo que liga o seu PC ao monitor e volte a ligá-lo.
2. Desligue quaisquer dispositivos não essenciais do seu PC (tais como adaptadores ou docas).

**Se instalou recentemente uma atualização no seu PC, pode reverter o controlador de exibição:**

1. Selecione **Iniciar,** digitar **o gestor do dispositivo** e selecione Device **Manager** a partir dos resultados.
2. Expanda a secção **de adaptadores do Ecrã,** clique com o botão direito do adaptador de ecrã e selecione **Propriedades**.
3. Navegue no **separador Condutor** e selecione **Roll Back Driver**. <br>
Nota: Se isto não estiver disponível ou estiver acinzentado, selecione **Não** das opções abaixo para passar para o passo seguinte.
4. Pode ser necessário reiniciar o seu PC antes que estas alterações entrem em vigor.

**Desinstalar e reinstalar o controlador de exibição:**

1. Selecione **Iniciar,** digitar **o gestor do dispositivo** e selecione Device **Manager** a partir dos resultados.
2. Expanda a secção **de adaptadores do Ecrã,** clique com o botão direito do adaptador de ecrã e selecione **o dispositivo Desinstalar**. 
3. Selecione a caixa ao lado **de Eliminar o software do controlador para este dispositivo** e selecione **Desinstalar**.<br>
Nota: Pode ser-lhe pedido que reinicie o computador nesta fase. Certifique-se de que anota as restantes instruções antes de reiniciar.
4. Abra o Gestor de Dispositivos novamente.
5. Expanda a secção **de adaptadores do Ecrã,** clique com o botão direito no adaptador de ecrã e selecione **'Actualizar' Driver**.
6. Selecione **Procurar automaticamente para atualizar o software do controlador** e siga as instruções de instalação.