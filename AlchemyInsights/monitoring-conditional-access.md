---
title: Controlo de acesso condicional
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 756c5e98ed3e9cedd0152b5747ea6bf1ed31778e
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/12/2019
ms.locfileid: "29902368"
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
    
Ler mais: [como dispositivos de Monitor de acesso condicional](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

