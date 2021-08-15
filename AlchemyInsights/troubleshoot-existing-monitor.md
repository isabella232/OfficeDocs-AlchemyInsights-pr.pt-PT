---
title: Remoção de problemas de um monitor existente
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
ms.openlocfilehash: 2ecfb4e90f2d58654ec43a35e901ea4421e0e94fa95995ef890abc8af2d99ec7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53981088"
---
# <a name="troubleshoot-an-existing-monitor"></a>Remoção de problemas de um monitor existente

Experimente estas soluções para remova um monitor. 

**Aumente o ecrã do monitor:**

Prima as seguintes teclas ao mesmo tempo: tecla Windows + Ctrl + Shift + B. Esta ação irá atualizar a comunicação com o controlador da sua placa gráfica. Os monitores ficarão intermitentemente momentaneamente e voltarão após alguns segundos.

**Remova o hardware do monitor:**

1. Desligue o cabo que liga o PC ao monitor e ligue-o novamente.
2. Desligue todos os dispositivos não essenciais do PC (como adaptadores ou docks).

**Se instalou recentemente uma atualização no seu PC, pode recuar o controlador de visualização:**

1. **Selecione Iniciar**, escreva **gestor de dispositivos** e selecione **Gestor de** Dispositivos a partir dos resultados.
2. Expanda a **secção Adaptadores de visualização,** clique com o botão direito do rato no adaptador de ecrã e selecione **Propriedades.**
3. Navegue para o **separador Controlador e** selecione **Roll Back Driver**. <br>
Nota: se esta opção não estiver disponível  ou estiver a cinzento, selecione Não nas opções abaixo para avançar para o passo seguinte.
4. Poderá ter de reiniciar o PC antes que estas alterações entrem em vigor.

**Desinstale e reinstale o controlador de visualização:**

1. **Selecione Iniciar**, escreva **gestor de dispositivos** e selecione **Gestor de** Dispositivos a partir dos resultados.
2. Expanda a **secção Adaptadores de visualização,** clique com o botão direito do rato no adaptador de ecrã e selecione Desinstalar **dispositivo**. 
3. Selecione a caixa junto **a Eliminar o software do controlador deste dispositivo e selecione** **Desinstalar**.<br>
Nota: nesta fase, poderá ser-lhe pedido para reiniciar o computador. Certifique-se de que anota as instruções restantes antes de reiniciar.
4. Abra novamente o Gestor de Dispositivos.
5. Expanda a **secção Adaptadores de visualização,** clique com o botão direito do rato no adaptador de visualização e selecione **Atualizar Controlador**.
6. **Selecione Procurar automaticamente software do controlador de atualização** e siga as instruções de instalação.