---
title: Monitorização existente da resolução de problemas
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: 2dc9a24c1d0d808e26733738cedbc32d513926a0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690722"
---
# <a name="troubleshoot-an-existing-monitor"></a>Resolução de problemas de um monitor existente

Experimente estas soluções para resolver problemas num monitor. 

**Refresque o visor do monitor:**

Prima as seguintes teclas ao mesmo tempo: Tecla do Windows + Ctrl + Shift + B. Isto irá refrescar a comunicação com o seu controlador gráfico. Os seus monitores piscarão momentaneamente e voltarão após alguns segundos.

**Hardware do monitor de resolução de problemas:**

1. Desligue o cabo que liga o seu PC ao monitor e volte a ligá-lo.
2. Desligue quaisquer dispositivos não essenciais do seu PC (tais como adaptadores ou docas).

**Se instalou recentemente uma atualização no seu PC, pode reverter o controlador de exibição:**

1. Selecione **Iniciar,** digitar **o gestor do dispositivo**e selecione Device **Manager** a partir dos resultados.
2. Expanda a secção **de adaptadores do Ecrã,** clique com o botão direito do adaptador de ecrã e selecione **Propriedades**.
3. Navegue no **separador Condutor** e selecione **Roll Back Driver**. <br>
Nota: Se isto não estiver disponível ou estiver acinzentado, selecione **Não** das opções abaixo para passar para o passo seguinte.
4. Pode ser necessário reiniciar o seu PC antes que estas alterações entrem em vigor.

**Desinstalar e reinstalar o controlador de exibição:**

1. Selecione **Iniciar,** digitar **o gestor do dispositivo**e selecione Device **Manager** a partir dos resultados.
2. Expanda a secção **de adaptadores do Ecrã,** clique com o botão direito do adaptador de ecrã e selecione **o dispositivo Desinstalar**. 
3. Selecione a caixa ao lado **de Eliminar o software do controlador para este dispositivo** e selecione **Desinstalar**.<br>
Nota: Pode ser-lhe pedido que reinicie o computador nesta fase. Certifique-se de que anota as restantes instruções antes de reiniciar.
4. Abra o Gestor de Dispositivos novamente.
5. Expanda a secção **de adaptadores do Ecrã,** clique com o botão direito no adaptador de ecrã e selecione **'Actualizar' Driver**.
6. Selecione **Procurar automaticamente para atualizar o software do controlador** e siga as instruções de instalação.