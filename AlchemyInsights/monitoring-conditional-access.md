---
title: Monitorização do Acesso Condicional
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 8b76d58791408037b5704b421d7afa166e3ea0be
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713729"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Monitorização do Acesso Condicional para Troca

Os utilizadores visados com acesso condicional receberão um e-mail de notificação se não cumprirem os requisitos de acesso da sua organização. Para resolver, recomendamos uma ou mais das seguintes soluções:
  
- Se o dispositivo for presumivelmente matriculado, aconselhe o utilizador a recorrer à aplicação Portal da Empresa e a verificar se aparece no Portal da Empresa. Se não o fizer, o utilizador deve inscrever o dispositivo.
    
- No portal Azure vá à **conformidade do Dispositivo Intune. \> ** Sob **o monitor** clique cumprimento do **dispositivo**. Consulte o relatório de conformidade do dispositivo para verificar se o dispositivo do utilizador está marcado como conforme. 
    
- No portal Azure vá à **conformidade do Dispositivo Intune. \> ** Em **'Gerir',** clique em **Políticas**. Na lista de políticas de conformidade, verifique se um perfil é atribuído ao dispositivo do utilizador. Se nenhum perfil for atribuído, então intune não será capaz de confirmar o estado de conformidade do dispositivo. 
    
- Editar a atribuição de acesso condicional do utilizador.
    
1. No portal Azure aceda a **Intune \> Políticas de acesso \> Condicional**
    
2. Selecione uma política da lista
    
3. Clique em **Utilizadores e grupos**
    
4. Para direcionar uma certa política para alguém, adicione-os à lista **de Incluir.** Para garantir que uma pessoa seja omitida da política, adicione-a à lista **de Excluir.** 
    
Leia mais: [Como monitorizar dispositivos](https://docs.microsoft.com/intune/conditional-access-exchange-monitor) de acesso condicional
  

