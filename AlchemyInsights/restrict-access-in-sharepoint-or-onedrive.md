---
title: Restringir o acesso no SharePoint ou OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: b6be074ed5f7e83f8196ca3fe90252673896569f
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/24/2019
ms.locfileid: "29483997"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="f35c7-102">Restringir o acesso no SharePoint ou OneDrive</span><span class="sxs-lookup"><span data-stu-id="f35c7-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="f35c7-p101">No SharePoint e OneDrive, restrinja o acesso a itens como ficheiros, pastas e listas concedendo acesso apenas a grupos ou indivíduos que pretende ter acesso. Por predefinição, as permissões no SharePoint são herdadas da cópia de segurança mais elevada na hierarquia. Para um ficheiro herda as suas permissões da pasta herda as suas permissões da biblioteca herda as suas permissões do site.</span><span class="sxs-lookup"><span data-stu-id="f35c7-p101">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access. By default, permissions in SharePoint are inherited from higher up in the hierarchy. So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="f35c7-p102">Pode partilhar um nível superior (tal como através da partilha de um site inteiro) e, em seguida, interromper a herança, se não pretender partilhar todos os itens no site. No entanto, não recomendamos este que torna a manter as permissões mais complexas e confusas no futuro. Eis o que pode fazer em vez disso:</span><span class="sxs-lookup"><span data-stu-id="f35c7-p102">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site. However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future. Here's what you could do instead:</span></span>
  
- <span data-ttu-id="f35c7-109">Se, por exemplo, pretender partilhar todo o conteúdo de uma pasta, excepto para um ficheiro, mova esse ficheiro para uma nova localização que não está partilhada.</span><span class="sxs-lookup"><span data-stu-id="f35c7-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="f35c7-110">Se tiver duas subpastas numa pasta e pretender partilhar uma subpasta com grupos A e B e permitir apenas acesso de grupo para a subpasta segundo, partilhar a pasta principal com o grupo e adicionar o grupo B para a primeira subpasta.</span><span class="sxs-lookup"><span data-stu-id="f35c7-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="f35c7-111">Parar de partilhar um ficheiro ou pasta</span><span class="sxs-lookup"><span data-stu-id="f35c7-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

