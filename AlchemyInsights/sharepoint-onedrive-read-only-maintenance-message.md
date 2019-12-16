---
title: Leia-somente para a mensagem de manutenção ao tentar usar sharepoint ou onedrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 02cf1aa7abae365a3d317af9e785648d1c1517e1
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051292"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Leia-somente para a mensagem de manutenção ao tentar usar sharepoint ou onedrive

Os usuários podem receber uma mensagem **de leitura somente para manutenção** ao tentar usar o SharePoint ou o OneDrive para um dos seguintes cenários. 

-   Uma atividade de manutenção planejada ou ativa.  Verifique se eles, navegando para o Centro de [Mensagens](https://portal.office.com/adminportal/home#/messagecenter).
-   Um incidente de serviço ativo de alta prioridade que pode estar ocorrendo. Verifique se há avisos/incidentes navegando para o [Serviço de Saúde.](https://portal.office.com/adminportal/home#/servicehealth)
-   Um cenário de recuperação de auto-cura menor que poderia estar acontecendo devido a quaisquer eventos inesperados nos servidores que podem durar menos de 30 min ou assim. 
    
    Não há mensagens do Centro de Mensagens ou de Saúde de Serviço para essas pequenas recuperações, mas você deve estar de volta ao normal muito em breve.

Em poucas ocasiões, observamos que um dos três cenários listados acima foi a causa, e o serviço foi restaurado, mas o cache do navegador de usuários não foi esclarecido.

Por favor, tente limpar o cache do navegador antes de navegar para o site.

1. No navegador Microsoft Edge, selecione **configurações**e selecione **privacidade e segurança.**
2. Em **navegação clara,** **selecione escolha o que limpar.**
3. Selecione **cookies e economizou dados**do site, e **selecione Clear**.

>[!Note] 
> Essas etapas podem diferir ao usar outros navegadores, como o Mozilla Firefox ou o Google Chrome.

>[!Note] 
> Outra opção seria abrir seu site SharePoint ou OneDrive em uma nova janela InPrivate.