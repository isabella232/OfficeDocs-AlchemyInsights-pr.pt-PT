---
title: Controlo de acesso condicional
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 06307b57475e8828e6d4e5e01625d5100576f12b
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/15/2019
ms.locfileid: "28306393"
---
# <a name="monitoring-conditional-access"></a>Controlo de acesso condicional

Os utilizadores visados com acesso condicional irão receber uma notificação por correio electrónico se não satisfizerem os requisitos de acesso de sua organização. Para resolver, recomenda-se um ou mais das seguintes soluções:
  
- Se presume-se que o dispositivo ser inscrito, aconselhará o utilizador para ir para a aplicação de Portal da empresa e certifique-se de que é apresentada no Portal da empresa. Caso contrário, o utilizador deverá inscrever-se o dispositivo.
    
- No Azure portal Ir para **Intune \> conformidade de dispositivo**. No **Monitor** , clique em **cumprimento do dispositivo**. Ver o relatório de conformidade do dispositivo para verificar que o dispositivo do utilizador está marcado como compatível. 
    
- No Azure portal Ir para **Intune \> conformidade de dispositivo**. Em **Gerir**, clique em **políticas**. Na lista de políticas de conformidade, certifique-se de que é atribuído um perfil de dispositivo do utilizador. Não se for atribuído nenhum perfil, em seguida, Intune não será possível confirmar o estado da conformidade do dispositivo. 
    
- Edite atribuição de acesso condicional do utilizador.
    
1. No Azure portal Ir para **Intune \> acesso condicional \> políticas**
    
2. Seleccione uma política a partir da lista
    
3. Clique em **utilizadores e grupos**
    
4. Para direccionar uma determinada política a alguém, tem de adicioná-los à lista de **inclusão** . Para assegurar que uma pessoa for omitida da política, adicioná-los à lista de **exclusão** . 
    
Ler mais: [como dispositivos de Monitor de acesso condicional](https://docs.microsoft.com/en-us/intune/conditional-access-exchange-monitor)
  

