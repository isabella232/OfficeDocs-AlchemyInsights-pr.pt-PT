---
title: A ação Abrir com o Explorador não funciona
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 2ba6f08b40dd194bf1ffd9a455a134a2fc553b51
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321872"
---
# <a name="open-with-explorer-isnt-working"></a>A ação Abrir com o Explorador não está a funcionar

Se as instruções  Abrir com o **Explorador** ou Ver no Explorador de  Ficheiros não funcionarem, certifique-se de que o serviço WebClient está definido para A executar ao seguir os passos abaixo. Por exemplo, poderá demorar muito tempo a abrir uma biblioteca de uma biblioteca do SharePoint OneDrive quando o serviço não estiver em execução. 
  
1. Na caixa de Windows, escreva executar, selecione a aplicação Executar ambiente de trabalho, escreva services.msc e, em seguida, selecione **Enter.**
    
2. Desloque-se para baixo até ao serviço WebClient e verifique **a coluna** Estado. Se o estado do serviço WebClient não estiver em **Execução**, faça duplo clique no serviço, clique em **Iniciar** e, em seguida, clique em **OK.** Se necessário, ative o serviço ao selecionar **Manual** **ou** Automático na caixa Tipo de **arranque.** 
    
**Nota:** para refletir problemas que abrem no Explorador de Ficheiros, consulte [Abrir no Explorador.](https://go.microsoft.com/fwlink/?linkid=871665) Explore a sincronização como uma alternativa melhor: [Sincronização de ficheiros do SharePoint com o novo Sincronização do OneDrive cliente](https://go.microsoft.com/fwlink/?linkid=871666). 
  

