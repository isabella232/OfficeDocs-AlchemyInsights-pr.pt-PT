---
title: Restringir o acesso no SharePoint ou OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: b7b68df2ae24b09fe9b01bd67c31a89e37f284a512bc1ecb097ef52fae5ae7d6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54075051"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Restringir o acesso no SharePoint ou OneDrive

No SharePoint e no OneDrive, pode restringir o acesso a itens como ficheiros, pastas e listas ao conceder acesso apenas a grupos ou pessoas a quem pretende conceder acesso. Por predefinição, as permissões no SharePoint são herdadas de um valor superior na hierarquia. Assim, um ficheiro herda as permissões da pasta, que herda as permissões da biblioteca, o que herda as permissões do site.
  
Pode partilhar num nível mais elevado (por exemplo, ao partilhar um site inteiro) e, em seguida, interromper a herança se não quiser partilhar todos os itens no site. No entanto, não o recomendamos, uma vez que torna a manutenção das permissões mais complexa e confusa no futuro. Em alternativa, eis o que pode fazer:
  
- Por exemplo, se quiser partilhar todos os conteúdos de uma pasta exceto um ficheiro, mova esse ficheiro para uma nova localização que não seja partilhada.
    
- Se tiver duas subpastas numa pasta e quiser partilhar uma subpasta com os grupos A e B e permitir apenas o acesso A à segunda subpasta, partilhe a pasta principal com o grupo A e adicione o grupo B à primeira subpasta.
    
[Parar de partilhar um ficheiro ou pasta ](https://go.microsoft.com/fwlink/?linkid=2008861)
  

