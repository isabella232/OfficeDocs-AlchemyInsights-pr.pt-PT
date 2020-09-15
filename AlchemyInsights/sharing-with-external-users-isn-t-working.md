---
title: Partilhar com utilizadores externos não está a funcionar
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: bd3a6c0d7206801ff76be121c4878b8343cc9886
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691586"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Corrigir problemas de partilha de conteúdo do SharePoint com utilizadores externos

Certifique-se de que a partilha externa está ligada à sua organização:
  
1. Aceda à [ &amp; página de suplementos de serviços no centro de administração Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)e clique em **Sites**.
    
2. Certifique-se de que a definição está virada para "Ligado". Se for selecionado "Apenas utilizadores externos existentes", certifique-se de que o utilizador externo está listado no centro de administração microsoft 365.
    
Certifique-se de que a partilha externa foi ligada para o site. Para uma coleção de site clássico:
  
1. No novo centro de administração do SharePoint, no painel esquerdo, clique nos **sites**.
    
2. Selecione o site ou sites, e na fita, clique em **Partilhar**.
    
Para um site de equipa que pertence a um grupo Microsoft 365, ou um site de comunicação:
  
- Estes novos tipos de sites têm a mesma definição de partilha que a configuração da organização, a menos que a configuração em toda a organização permita partilhar ficheiros usando links que não requerem o acesso. Neste caso, os sites permitem a partilha com utilizadores externos novos e existentes que se inscrevem. Para alterar a definição para sites específicos, utilize o novo centro de administração sharePoint ou PowerShell. [Saiba mais](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> A definição de partilha externa para qualquer site pode ser mais restritiva do que a configuração em toda a organização, mas não mais permissiva do que a configuração em toda a organização. 
  

