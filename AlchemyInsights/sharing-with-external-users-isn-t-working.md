---
title: Compartilhar com usuários externos não está funcionando
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: d4c8fc75ff8db2319b88a20bea9b3ee661f2e36e
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/18/2019
ms.locfileid: "36502242"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Corrigir problemas de compartilhamento de conteúdo do SharePoint com usuários externos

Certifique-se de que o compartilhamento externo esteja ativado para sua organização:
  
1. Vá para a [página &amp; de suplementos de serviços no centro de administração do Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)e clique em **sites**.
    
2. Certifique-se de que a definição está virada para "ligado". Se "somente usuários externos existentes" estiver selecionado, certifique-se de que o usuário externo está listado no centro de administração do Microsoft 365.
    
Certifique-se de que o compartilhamento externo esteja ativado para o site. Para um conjunto de sites clássico:
  
1. No novo centro de administração do SharePoint, no painel esquerdo, clique em **sites**.
    
2. Selecione o site ou sites e, na faixa de opções, clique em **compartilhamento**.
    
Para um site de equipe que pertence a um grupo do Office 365 ou um site de comunicação:
  
- Esses novos tipos de site têm a mesma configuração de compartilhamento que a configuração de toda a organização, a menos que a configuração de toda a organização permita o compartilhamento de arquivos usando links que não exijam login. Nesse caso, os sites permitem o compartilhamento com usuários externos novos e existentes que fizerem login. Para alterar a configuração de sites específicos, use o novo centro de administração do SharePoint ou o PowerShell. [Saiba mais](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> A configuração de compartilhamento externo para qualquer site pode ser mais restritiva do que a configuração de toda a organização, mas não mais permissiva do que a configuração de toda a organização. 
  

