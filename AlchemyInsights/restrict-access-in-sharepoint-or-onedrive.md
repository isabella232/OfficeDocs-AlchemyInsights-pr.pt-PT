---
title: Restringir o acesso no SharePoint ou no OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e5458226fe33bd5cb3da1f608fb113b888fbfd16
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/18/2019
ms.locfileid: "36551462"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Restringir o acesso no SharePoint ou no OneDrive

No SharePoint e no OneDrive, você restringe o acesso a itens como arquivos, pastas e listas concedendo acesso somente a grupos ou indivíduos que você deseja ter acesso. Por padrão, as permissões no SharePoint são herdadas mais acima na hierarquia. Portanto, um arquivo herda suas permissões da pasta, que herda suas permissões da biblioteca, que herda suas permissões do site.
  
Você pode compartilhar em um nível mais alto (por exemplo, compartilhando um site inteiro) e, em seguida, interromper a herança se você não quiser compartilhar todos os itens no site. No entanto, não recomendamos isso porque torna a manutenção das permissões mais complexas e confusas no futuro. Aqui está o que você poderia fazer em vez disso:
  
- Se, por exemplo, você quiser compartilhar todo o conteúdo de uma pasta, exceto por um arquivo, mova esse arquivo para um novo local que não seja compartilhado.
    
- Se tiver duas subpastas numa pasta e pretender partilhar uma subpasta com grupos A e B e permitir apenas o grupo a acesso à segunda subpasta, partilhe a pasta principal com o grupo A e adicione o grupo B à primeira subpasta.
    
[Interromper o compartilhamento de um arquivo ou pasta](https://go.microsoft.com/fwlink/?linkid=2008861)
  

