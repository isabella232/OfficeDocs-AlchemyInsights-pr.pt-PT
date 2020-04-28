---
title: Partilhar com utilizadores externos não está a funcionar
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 37da77c73b3abbdcf9cb2b9c4c43f31eea3c0a49
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/27/2020
ms.locfileid: "43913013"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Corrigir problemas de partilha de conteúdo do SharePoint com utilizadores externos

Certifique-se de que a partilha externa está ligada para a sua organização:
  
1. Vá à página de [add-ins dos Serviços &amp; no centro de administração da Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), e clique em **Sites**.
    
2. Certifique-se de que a definição está virada para "On". Se "Apenas forem selecionados utilizadores externos existentes", certifique-se de que o utilizador externo está listado no centro de administração da Microsoft 365.
    
Certifique-se de que a partilha externa foi ligada para o site. Para uma coleção clássica do site:
  
1. No novo centro de administração do SharePoint, no painel esquerdo, clique **em sites**.
    
2. Selecione o site ou os sites e na fita, clique em **Partilhar**.
    
Para um site de equipa que pertence a um grupo Microsoft 365, ou a um site de comunicação:
  
- Estes novos tipos de sites têm a mesma definição de partilha que a sua configuração em toda a organização, a menos que a definição em toda a organização permita a partilha de ficheiros usando links que não requerem iniciar sessão. Neste caso, os sites permitem a partilha com utilizadores externos novos e existentes que se inscrevam. Para alterar a definição para sites específicos, utilize o novo centro de administração do SharePoint ou o PowerShell. [Saiba mais](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> O cenário de partilha externa para qualquer site pode ser mais restritivo do que o ambiente em toda a organização, mas não mais permissivo do que o ambiente em toda a organização. 
  

