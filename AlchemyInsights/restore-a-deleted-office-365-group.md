---
title: Restaurar um grupo Microsoft 365 eliminado
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: b72b7c93ce9fe1b90d1608811b0eeabc8aec1363
ms.sourcegitcommit: a5edaaefdc56f8d5c8220a335f4e8228e2de4ee0
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/08/2021
ms.locfileid: "51645142"
---
# <a name="restore-a-deleted-microsoft-365-group"></a><span data-ttu-id="3d7e6-102">Restaurar um grupo Microsoft 365 eliminado</span><span class="sxs-lookup"><span data-stu-id="3d7e6-102">Restore a deleted Microsoft 365 group</span></span>

<span data-ttu-id="3d7e6-103">Pode restaurar um grupo Microsoft 365 ou Microsoft Teams eliminados no prazo de 30 dias a partir da eliminação.</span><span class="sxs-lookup"><span data-stu-id="3d7e6-103">You can restore a deleted Microsoft 365 group or Microsoft Teams within 30 days from the deletion.</span></span>

1. <span data-ttu-id="3d7e6-104">Vá ao [centro de administração microsoft 365](https://aka.ms/RestoreDeletedGroup) para iniciar sessão numa lista de vocês são os grupos e equipas eliminados.</span><span class="sxs-lookup"><span data-stu-id="3d7e6-104">Go to the [Microsoft 365 admin center](https://aka.ms/RestoreDeletedGroup) to log in to a list of your the deleted groups and teams.</span></span>

    <span data-ttu-id="3d7e6-105">**Nota:** Faça login usando a conta que é atribuída ao administrador do inquilino ou à função de administrador de grupos.</span><span class="sxs-lookup"><span data-stu-id="3d7e6-105">**Note:** Log in using the account that is assigned to either the tenant administrator or the groups admin role.</span></span>

1. <span data-ttu-id="3d7e6-106">Selecione o grupo/equipas do Microsoft 365 eliminados para ser restaurado e clique em **restaurar o grupo**.</span><span class="sxs-lookup"><span data-stu-id="3d7e6-106">Select the deleted Microsoft 365 group/Teams to be restored and click **restore group**.</span></span>

    <span data-ttu-id="3d7e6-107">Se o grupo não puder ser restaurado por causa de um endereço SMTP conflituoso, use o seguinte comando para encontrar o objeto que está a causar conflito e remover o endereço SMTP:</span><span class="sxs-lookup"><span data-stu-id="3d7e6-107">If the group can't be restored because of a conflicting SMTP address, use following command to find the object that’s causing conflict and remove the SMTP address:</span></span>

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    <span data-ttu-id="3d7e6-108">**Nota:** Em alguns casos, pode levar até 24 horas para o grupo e todos os seus dados serem restaurados.</span><span class="sxs-lookup"><span data-stu-id="3d7e6-108">**Note:** In some cases, it might take as long as 24 hours for the group and all of its data to be restored.</span></span>

    <span data-ttu-id="3d7e6-109">Para obter mais informações ou para aprender a restaurar grupos usando o PowerShell, consulte [Restaurar um grupo Microsoft 365 eliminado](https://go.microsoft.com/fwlink/?linkid=867802).</span><span class="sxs-lookup"><span data-stu-id="3d7e6-109">For more info, or to learn how to restore groups using PowerShell, see [Restore a deleted Microsoft 365 group](https://go.microsoft.com/fwlink/?linkid=867802).</span></span>