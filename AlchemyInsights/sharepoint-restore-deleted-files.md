---
title: Restaurar um ficheiro ou pasta eliminado
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ba1573a5-9f44-482b-8082-6f648f169449
ms.openlocfilehash: 8c7ce48f50b5c933ea15c23a486b99ad7a7f4d79
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707533"
---
# <a name="restore-a-deleted-file-or-folder"></a><span data-ttu-id="3efc9-102">Restaurar um ficheiro ou pasta eliminado</span><span class="sxs-lookup"><span data-stu-id="3efc9-102">Restore a deleted file or folder</span></span>

<span data-ttu-id="3efc9-103">O SharePoint Online conserva cópias de segurança de todos os conteúdos durante mais 14 dias após a eliminação.</span><span class="sxs-lookup"><span data-stu-id="3efc9-103">SharePoint Online retains backups of all content for 14 additional days beyond actual deletion.</span></span> <span data-ttu-id="3efc9-104">Se o conteúdo não puder ser restaurado através do "Reciclar" ou "Restaurar ficheiros", um administrador pode contactar o Microsoft Support para solicitar uma restauração dentro da janela de 14 dias.</span><span class="sxs-lookup"><span data-stu-id="3efc9-104">If content cannot be restored via the Recycle Bin or Files Restore, an administrator can contact Microsoft Support to request a restore any time inside the 14 day window.</span></span> <span data-ttu-id="3efc9-105">Só podem ser efetuados restauros de cópias de segurança para coleções de sites ou subsites, não para ficheiros, listas ou bibliotecas específicos.</span><span class="sxs-lookup"><span data-stu-id="3efc9-105">Restorations from backups can only be completed for site collections or sub-sites, not for specific files, lists, or libraries.</span></span>

<span data-ttu-id="3efc9-106">Quando elimina um item ou site do Sharepoint, este não é imediatamente removido.</span><span class="sxs-lookup"><span data-stu-id="3efc9-106">When you delete an item or site from Sharepoint, it isn't immediately removed.</span></span> <span data-ttu-id="3efc9-107">Os itens eliminados ficam durante um período de tempo na reciclagem.</span><span class="sxs-lookup"><span data-stu-id="3efc9-107">Deleted items go into the recycle bin for a period of time.</span></span> <span data-ttu-id="3efc9-108">Durante este período, pode restaurar os itens que eliminou para a respetiva localização original.</span><span class="sxs-lookup"><span data-stu-id="3efc9-108">During that time, you can restore the items you deleted to their original location.</span></span> <span data-ttu-id="3efc9-109">Para obter mais informações, visite as ligações abaixo.</span><span class="sxs-lookup"><span data-stu-id="3efc9-109">For more information, please visit the links below.</span></span>

<span data-ttu-id="3efc9-110">[Restaurar os itens no Caixote do Lixo de um site do SharePoint.](https://support.microsoft.com/office/restore-items-in-the-recycle-bin-that-were-deleted-from-sharepoint-or-teams-6df466b6-55f2-4898-8d6e-c0dff851a0be)</span><span class="sxs-lookup"><span data-stu-id="3efc9-110">[Restore items in the Recycle Bin of a SharePoint site](https://support.microsoft.com/office/restore-items-in-the-recycle-bin-that-were-deleted-from-sharepoint-or-teams-6df466b6-55f2-4898-8d6e-c0dff851a0be).</span></span>

[<span data-ttu-id="3efc9-111">Restaurar ficheiros ou pastas eliminadas no OneDrive</span><span class="sxs-lookup"><span data-stu-id="3efc9-111">Restore deleted files or folders in OneDrive</span></span>](https://support.office.com/article/Restore-deleted-files-or-folders-in-OneDrive-949ada80-0026-4db3-a953-c99083e6a84f)

[<span data-ttu-id="3efc9-112">Restaurar uma coleção de site eliminada (Incluindo grupo, comunicação e outros sites)</span><span class="sxs-lookup"><span data-stu-id="3efc9-112">Restore a deleted site collection (Including group, communication and other sites)</span></span>](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)

[<span data-ttu-id="3efc9-113">Restaurar um site OneDrive eliminado</span><span class="sxs-lookup"><span data-stu-id="3efc9-113">Restore a deleted OneDrive site</span></span>](https://docs.microsoft.com/onedrive/restore-deleted-onedrive)

<span data-ttu-id="3efc9-114">Para ações de reciclagem a granel, os administradores podem considerar a utilização [do Sharepoint Online PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span><span class="sxs-lookup"><span data-stu-id="3efc9-114">For bulk recycle bin actions, admins may consider using [Sharepoint Online PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span></span>

<span data-ttu-id="3efc9-115">**Funcionalidade de Restauro de Ficheiros**</span><span class="sxs-lookup"><span data-stu-id="3efc9-115">**Files Restore feature**</span></span>

<span data-ttu-id="3efc9-116">Se muitos dos seus ficheiros OneDrive ou SharePoint forem eliminados, substituídos, corrompidos ou infetados por malware, pode restaurar toda a sua biblioteca OneDrive ou SharePoint para uma vez anterior utilizando a funcionalidade de restauro de ficheiros.</span><span class="sxs-lookup"><span data-stu-id="3efc9-116">If lots of your OneDrive or SharePoint files get deleted, overwritten, corrupted, or infected by malware, you can restore your entire OneDrive or SharePoint library to a previous time using the files restore feature.</span></span>

[<span data-ttu-id="3efc9-117">Restaurar uma biblioteca do OneDrive</span><span class="sxs-lookup"><span data-stu-id="3efc9-117">Restore a OneDrive library</span></span>](https://support.office.com/article/restore-your-onedrive-fa231298-759d-41cf-bcd0-25ac53eb8a15)

[<span data-ttu-id="3efc9-118">Restaurar uma biblioteca de documentos</span><span class="sxs-lookup"><span data-stu-id="3efc9-118">Restore a Document library</span></span>](https://support.office.com/article/restore-a-document-library-317791c3-8bd0-4dfd-8254-3ca90883d39a)

