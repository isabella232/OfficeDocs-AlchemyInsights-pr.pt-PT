---
title: Restringir o acesso no SharePoint ou no OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: d8be1eb5bdcd0b5b08ddad32a45b6282c788c26a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720693"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Restringir o acesso no SharePoint ou no OneDrive

No SharePoint e no OneDrive, restringe o acesso a itens como ficheiros, pastas e listas, concedendo acesso apenas a grupos ou indivíduos a que pretende ter acesso. Por padrão, as permissões no SharePoint são herdadas do alto da hierarquia. Assim, um ficheiro herda as suas permissões da pasta, que herda as suas permissões da biblioteca, que herda as suas permissões do site.
  
Você pode compartilhar a um nível mais alto (como por exemplo, compartilhando um site inteiro) e, em seguida, quebrar a herança se você não quiser compartilhar todos os itens no site. No entanto, não recomendamos isto porque torna a manutenção das permissões mais complexa e confusa no futuro. Eis o que pode fazer em vez disso:
  
- Se, por exemplo, quiser partilhar todo o conteúdo de uma pasta, exceto um ficheiro, mova esse ficheiro para um novo local que não seja partilhado.
    
- Se tiver duas sub-dobras numa pasta e quiser partilhar uma sub-dobradura com os grupos A e B e permitir apenas o acesso do grupo A à segunda sub-dobra, partilhe a pasta dos pais com o grupo A e adicione o grupo B à primeira sub-dobra.
    
[Pare de partilhar um ficheiro ou pasta ](https://go.microsoft.com/fwlink/?linkid=2008861)
  

