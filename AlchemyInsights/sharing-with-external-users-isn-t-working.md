---
title: A partilha com utilizadores externos não está a funcionar
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
ms.openlocfilehash: 02d79c1b1e112eb41e8c60ffa2ef28e429f76ada
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58304380"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Corrigir problemas ao partilhar conteúdos do SharePoint com utilizadores externos

Certifique-se de que a partilha externa está adada para a sua organização:
  
1. Vá para [a página serviços de &amp; add-ins na centro de administração do Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)e clique em **Sites**.
    
2. Certifique-se de que a definição está selecta para "Ação". Se a opção "Apenas utilizadores externos existentes" estiver selecionada, certifique-se de que o utilizador externo está listado na centro de administração do Microsoft 365.
    
Certifique-se de que a partilha externa está atalhou para o site. Para uma coleção de site clássica:
  
1. No novo centro de administração do SharePoint, no painel esquerdo, clique em **sites**.
    
2. Selecione o site ou sites e, no fita, clique em **Partilha.**
    
Para um site de equipa que pertence a um Microsoft 365 de equipa ou a um site de comunicação:
  
- Estes novos tipos de site têm a mesma definição de partilha que a definição para toda a organização, a menos que a definição para toda a organização permita a partilha de ficheiros através de ligações que não necessitam de o fazer. Neste caso, os sites permitem a partilha com utilizadores externos novos e existentes que inscreveram a sua conta. Para alterar a definição de sites específicos, utilize o novo centro de administração do SharePoint ou o PowerShell. [Saiba mais](https://go.microsoft.com/fwlink/?linkid=871863).
    
**Nota:** a definição de partilha externa de qualquer site pode ser mais restritiva do que a definição de toda a organização, mas não mais permissiva do que a definição ao nível da organização. 
  

