---
title: Remova problemas ao utilizar a ação Abrir com o Explorador
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
ms.openlocfilehash: 0cbcfb506295d5732f7109be7a103bbdef530a529c7408c6d9d45a7b38a89915
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54048167"
---
# <a name="fix-problems-with-open-with-explorer"></a>Corrigir problemas com a ação Abrir com o Explorador

Corrigimos problemas comuns ao abrir uma biblioteca de documentos no SharePoint ou OneDrive com **o comando Abrir com o Explorador:** 
  
- Utilize Internet Explorer 10 ou Internet Explorer 11. **A aplicação Open with Explorer** não é compatível com o Microsoft Edge, o Google Chrome, o Firefox entre outros. **A funcionalidade Abrir com o Explorador** está desativada em todos os browsers exceto o Internet Explorer. 
    
- **A vista Abrir com o** Explorador não está disponível na experiência moderna para bibliotecas do SharePoint. Em **alternativa, utilize a vista no Explorador de Ficheiros.** **Selecione Ver opções Ver** no \> **Explorador de Ficheiros**. A vista no Explorador de Ficheiros não é compatível com o Microsoft Edge, o Google Chrome, o Firefox entre outros. **Ver no Explorador de Ficheiros** apenas disponível no Internet Explorer. 
    
- Certifique-se de que o serviço WebClient está em execução. Na caixa de Windows, escreva executar, selecione a aplicação Executar ambiente de trabalho, escreva services.msc e, em seguida, prima Enter. Desloque-se para baixo até ao serviço WebClient e certifique-se de que **a** coluna Estado apresenta "A executar". Se isso não acontecer, faça duplo clique no serviço, clique em Iniciar **e,** em seguida, clique em **OK.** (Poderá ter de ativar primeiro o serviço ao selecionar **Manual** ou **Automático** na **caixa Tipo de arranque.)** 
    
> [!NOTE]
> Abrir uma biblioteca no Explorador de Ficheiros é útil se precisar de copiar ou mover múltiplos ficheiros e pastas uma vez, mas se quiser trabalhar regularmente na biblioteca, recomendamos que a mesma seja silenciada. Para refletir problemas que se abrem no Explorador de Ficheiros, [consulte Abrir no Explorador.](https://go.microsoft.com/fwlink/?linkid=871665) Para mais informações sobre como configurar a sincronização, consulte [Sincronização](https://go.microsoft.com/fwlink/?linkid=871666)de ficheiros do SharePoint com o novo Sincronização do OneDrive cliente .
  
Consulte o artigo Como utilizar o comando "Abrir com o [Explorador"](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) para remoção de problemas no SharePoint Online para obter mais informações. 
  

