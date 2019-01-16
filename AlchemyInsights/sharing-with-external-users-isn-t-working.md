---
title: Partilhar com utilizadores externos não funciona
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 305b3891e6c83e27b5c55c13757640e6e9d51a81
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/15/2019
ms.locfileid: "28305999"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Corrigir problemas de partilha do conteúdo do SharePoint com utilizadores externos

Certifique-se de partilha externa está activada para a sua organização:
  
1. Vá para o [Serviços de &amp; página de suplementos no Office 365 admin Centro](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)e clique em **Sites**.
    
2. Certifique-se que a definição é ligada como "On". Se estão seleccionados "Só utilizadores externos existentes", certifique-se o utilizador externo é listado no Centro de administração do Office 365.
    
Certifique-se externo partilha activada para o site. Para uma colecção de sites clássico:
  
1. No Centro de administração SharePoint clássico, no painel da esquerda, clique em **colecções de sites**.
    
2. Seleccione o local ou locais e no Friso, clique em **partilhar**.
    
Para um site de equipa que pertença a um grupo do Office 365 ou um site de comunicação:
  
- Estes novos tipos de site tem a mesma definição partilha como a definição de toda a organização, a menos que a definição de toda a organização permite a partilha de ficheiros a utilização de ligações que não requerem início de sessão. Neste caso, os sites permitem a partilha com utilizadores externos novos e existentes que iniciar sessão. Para alterar a definição para sites específicos, utilize o novo Centro de administração do SharePoint (pré-visualização) ou o PowerShell. [Mais informações](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> A definição de partilha externa para qualquer site pode ser mais restritiva do que a definição de toda a organização, mas não mais permissivas podem permitir que a definição de toda a organização. 
  

