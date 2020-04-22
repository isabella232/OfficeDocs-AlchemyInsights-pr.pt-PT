---
title: Aberto com Explorer não funciona
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: dc939a3451ff4fe95e4aa5a999839a2c532b398c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713045"
---
# <a name="open-with-explorer-isnt-working"></a>Abrir com explorador não está funcionando

Se **abrir com o Explorer** ou ver no File **Explorer** não funcionar, certifique-se de que o serviço WebClient está definido para **Executar** seguindo os passos abaixo. Por exemplo, pode levar muito tempo para abrir uma biblioteca SharePoint ou OneDrive quando o serviço não estiver em execução. 
  
1. Na caixa de pesquisa do Windows, digite, selecione a aplicação de ambiente de trabalho Run, escreva serviços.msc e, em seguida, selecione **Enter**.
    
2. Desloque-se até ao serviço WebClient e verifique a coluna **'Status'.** Se o estado de serviço do WebClient não estiver **a funcionar,** clique duas vezes no serviço, clique em **Iniciar**, e clique em **OK**. Ativar o serviço, se necessário, selecionando **manual** ou **automático** na caixa **do tipo Arranque.** 
    
> [!NOTE]
> Para resolver problemas de abertura no File Explorer, consulte [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Explore a sincronização como uma alternativa melhor: [Sync SharePoint ficheiros com o novo cliente sincronizado OneDrive](https://go.microsoft.com/fwlink/?linkid=871666). 
  

