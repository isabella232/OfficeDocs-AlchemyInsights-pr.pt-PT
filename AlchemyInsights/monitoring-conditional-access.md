---
title: Acesso Condicional de Monitorização
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 6083fc427e3791fdb0907198b525337a0c987c4e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702914"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Monitorização do Acesso Condicional para Troca

Os utilizadores direcionados com acesso condicional receberão um e-mail de notificação se não cumprirem os requisitos de acesso da sua organização. Para resolver, recomendamos uma ou mais das seguintes soluções:
  
- Caso se presuma que o dispositivo esteja matriculado, aconselhe o utilizador a recorrer à aplicação Portal da Empresa e verificar se aparece no Portal da Empresa. Se não o fizer, o utilizador deverá inscrever o dispositivo.
    
- No portal Azure aceda à ** \> conformidade do Dispositivo Intune**. No **Monitor** clique **na conformidade do dispositivo**. Consulte o relatório de conformidade do dispositivo para verificar se o dispositivo do utilizador está marcado como conforme. 
    
- No portal Azure aceda à ** \> conformidade do Dispositivo Intune**. Em **Gestão**, clique em **Políticas**. Na lista de políticas de conformidade, verifique se um perfil é atribuído ao dispositivo do seu utilizador. Se não for atribuído nenhum perfil, o Intune não poderá confirmar o estado de conformidade do dispositivo. 
    
- Editar a atribuição de acesso condicional do utilizador.
    
1. No portal Azure vai para Políticas de ** \> Acesso Condicionado \> Intune**
    
2. Selecione uma política da lista
    
3. Clique em **Utilizadores e grupos**
    
4. Para direcionar uma determinada política a alguém, adicione-a à lista **de incluir.** Para garantir que uma pessoa é omitida da apólice, adicione-a à lista **de exclusão.** 
    
Leia mais: [Como monitorizar dispositivos de acesso condicional](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

