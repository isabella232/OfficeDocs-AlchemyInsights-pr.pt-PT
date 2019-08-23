---
title: Restringir o acesso no SharePoint ou OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e5458226fe33bd5cb3da1f608fb113b888fbfd16
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551462"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="ad714-102">Restringir o acesso no SharePoint ou OneDrive</span><span class="sxs-lookup"><span data-stu-id="ad714-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="ad714-103">No SharePoint e OneDrive, restrinja o acesso a itens como ficheiros, pastas e listas concedendo acesso apenas a grupos ou indivíduos que pretende ter acesso.</span><span class="sxs-lookup"><span data-stu-id="ad714-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="ad714-104">Por predefinição, as permissões no SharePoint são herdadas da cópia de segurança mais elevada na hierarquia.</span><span class="sxs-lookup"><span data-stu-id="ad714-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="ad714-105">Para um ficheiro herda as suas permissões da pasta herda as suas permissões da biblioteca herda as suas permissões do site.</span><span class="sxs-lookup"><span data-stu-id="ad714-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="ad714-106">Pode partilhar um nível superior (tal como através da partilha de um site inteiro) e, em seguida, interromper a herança, se não pretender partilhar todos os itens no site.</span><span class="sxs-lookup"><span data-stu-id="ad714-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="ad714-107">No entanto, não recomendamos este que torna a manter as permissões mais complexas e confusas no futuro.</span><span class="sxs-lookup"><span data-stu-id="ad714-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="ad714-108">Eis o que pode fazer em vez disso:</span><span class="sxs-lookup"><span data-stu-id="ad714-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="ad714-109">Se, por exemplo, pretender partilhar todo o conteúdo de uma pasta, excepto para um ficheiro, mova esse ficheiro para uma nova localização que não está partilhada.</span><span class="sxs-lookup"><span data-stu-id="ad714-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="ad714-110">Se tiver duas subpastas numa pasta e pretender partilhar uma subpasta com grupos A e B e permitir apenas acesso de grupo para a subpasta segundo, partilhar a pasta principal com o grupo e adicionar o grupo B para a primeira subpasta.</span><span class="sxs-lookup"><span data-stu-id="ad714-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="ad714-111">Parar de partilhar um ficheiro ou pasta</span><span class="sxs-lookup"><span data-stu-id="ad714-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

