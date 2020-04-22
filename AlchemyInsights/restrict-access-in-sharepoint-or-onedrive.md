---
title: Restringir o acesso no SharePoint ou oneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: ed8e97b20c96a7b46995c969074cc4cef3a787d9
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43715895"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Restringir o acesso no SharePoint ou oneDrive

No SharePoint e no OneDrive, restringe o acesso a itens como ficheiros, pastas e listas, concedendo acesso apenas a grupos ou indivíduos que deseja ter acesso. Por padrão, as permissões no SharePoint são herdadas de um alto na hierarquia. Assim, um ficheiro herda as suas permissões da pasta, que herda as suas permissões da biblioteca, que herda as suas permissões a partir do site.
  
Você pode compartilhar a um nível mais alto (como por exemplo, partilhando um site inteiro) e, em seguida, quebrar a herança se você não quiser compartilhar todos os itens no site. No entanto, não recomendamos isto porque torna a manutenção das permissões mais complexas e confusas no futuro. Eis o que podias fazer em vez disso:
  
- Se, por exemplo, quiser partilhar todo o conteúdo de uma pasta, exceto um ficheiro, mude esse ficheiro para um novo local que não seja partilhado.
    
- Se tiver duas subpastas numa pasta e pretender partilhar uma subpasta com os grupos A e B e permitir apenas o acesso do grupo A à segunda subpasta, partilhe a pasta-mãe com o grupo A e adicione o grupo B à primeira subpasta.
    
[Pare de partilhar um ficheiro ou pasta](https://go.microsoft.com/fwlink/?linkid=2008861)
  

