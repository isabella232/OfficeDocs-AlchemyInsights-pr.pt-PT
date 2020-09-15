---
title: Problemas de resolução de problemas usando Open with Explorer
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: e7fe59b94d216d89c2f2f7100a3d8bf7a0b0196e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659069"
---
# <a name="fix-problems-with-open-with-explorer"></a>Corrigir problemas com Abrir com Explorador

Corrija problemas comuns com a abertura de uma biblioteca de documentos no SharePoint ou No OneDrive utilizando o comando **Open with Explorer:** 
  
- Utilize o Internet Explorer 10 ou o Internet Explorer 11. **Abrir com o Explorer** não é compatível com o Microsoft Edge, Google Chrome, Firefox e outros. **Aberto com o Explorer** é desativado em todos os navegadores, exceto no Internet Explorer. 
    
- **Open with Explorer** não está disponível na experiência moderna para bibliotecas SharePoint. Use **a vista no Explorador de Ficheiros** em vez disso. Selecione **Ver opções** \> **Ver no Explorador de Ficheiros**. A visualização no File Explorer não é compatível com o Microsoft Edge, Google Chrome, Firefox e outros. **Ver no File Explorer** disponível apenas no Internet Explorer. 
    
- Certifique-se de que o serviço WebClient está em funcionamento. Na caixa de pesquisa do Windows, escreva, selecione a aplicação de ambiente de trabalho Run, escreva serviços.msc e, em seguida, prima Enter. Desloque-se até ao serviço WebClient e certifique-se de que a coluna **Status** apresenta "Running". Se não o fizer, clique duas vezes no serviço, clique em **Iniciar**e, em seguida, clique **em OK**. (Pode ser necessário ativar primeiro o serviço selecionando **manual** ou **automático** na caixa **tipo Arranque.)** 
    
> [!NOTE]
> Abrir uma biblioteca no File Explorer é útil se precisar copiar ou mover vários ficheiros e pastas uma vez, mas se quiser trabalhar regularmente na biblioteca, recomendamos que o sincronize. Para resolver problemas de abertura no Explorador de Ficheiros, consulte [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Para obter informações sobre a configuração da sincronização, consulte [os ficheiros Sync SharePoint com o novo cliente de sincronização OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).
  
Consulte o artigo [Como utilizar o comando "Abrir com explorador" para resolver problemas no SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) para obter mais informações. 
  

