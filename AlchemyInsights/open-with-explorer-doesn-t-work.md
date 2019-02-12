---
title: Abrir com o Explorador não funciona
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: f788c3c626cdeb19970edb59563c59eea60e2992
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/12/2019
ms.locfileid: "29906815"
---
# <a name="open-with-explorer-isnt-working"></a>Abrir com o Explorer não está a funcionar

Se **Abrir com o Explorador** ou **vista do Explorador de ficheiros** não funciona certificar-se de que o serviço WebClient está definido para **ser executado** , seguindo os passos abaixo. Por exemplo, poderá demorar muito tempo a abrir uma biblioteca de SharePoint ou OneDrive quando o serviço não está em execução. 
  
1. Na caixa de procura do Windows, o tipo de executar, seleccione a executar aplicações de ambiente de trabalho, tipo msc e, em seguida, seleccione **Enter**.
    
2. Desloque-se para o serviço WebClient e verificar a coluna de **Estado** . Se o estado do serviço WebClient não está **em execução**, faça duplo clique sobre o serviço, clique em **Iniciar**e, em seguida, clique em **OK**. Active o serviço, se necessário, seleccionando o **Manual** ou **Automático** na caixa **tipo de arranque** . 
    
> [!NOTE]
> Para resolver problemas de abertura no Explorador de ficheiros, consulte [aberta no Explorador](https://go.microsoft.com/fwlink/?linkid=871665). Explorar sincronização como uma melhor alternativa: [ficheiros do SharePoint de sincronização com o novo cliente de sincronização de OneDrive](https://go.microsoft.com/fwlink/?linkid=871666). 
  

