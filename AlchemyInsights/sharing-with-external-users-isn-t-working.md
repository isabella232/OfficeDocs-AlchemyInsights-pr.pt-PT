---
title: Partilhar com utilizadores externos não funciona
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 20b538846997c021b6e88596a1e8aff401ea935b
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/12/2019
ms.locfileid: "29900893"
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
  

