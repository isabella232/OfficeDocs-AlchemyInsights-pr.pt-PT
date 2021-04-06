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
ms.openlocfilehash: caa2c8987eecb89bac3469bf9471847858cab0ba
ms.sourcegitcommit: ec99a3a2e1e6a13d9a829d65ad1692a607dc3a17
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/06/2021
ms.locfileid: "51597454"
---
# <a name="restore-a-deleted-microsoft-365-group"></a><span data-ttu-id="c635d-102">Restaurar um grupo Microsoft 365 eliminado</span><span class="sxs-lookup"><span data-stu-id="c635d-102">Restore a deleted Microsoft 365 group</span></span>

<span data-ttu-id="c635d-103">Pode restaurar um grupo Microsoft 365 ou Microsoft Teams eliminados no prazo de 30 dias a partir da eliminação.</span><span class="sxs-lookup"><span data-stu-id="c635d-103">You can restore a deleted Microsoft 365 group or Microsoft Teams within 30 days from the deletion.</span></span>

1. <span data-ttu-id="c635d-104">Vá ao [centro de administração microsoft 365](https://aka.ms/RestoreDeletedGroup) para iniciar sessão e listar os grupos e equipas eliminados.</span><span class="sxs-lookup"><span data-stu-id="c635d-104">Go to the [Microsoft 365 admin center](https://aka.ms/RestoreDeletedGroup) to log in and list the deleted groups and teams.</span></span>

    <span data-ttu-id="c635d-105">**Nota:** Faça login usando a conta que é atribuída ao administrador do inquilino ou à função de administrador de grupos.</span><span class="sxs-lookup"><span data-stu-id="c635d-105">**Note:** Log in using the account that is assigned to either the tenant administrator or the groups admin role.</span></span>

1. <span data-ttu-id="c635d-106">Selecione o grupo/equipas do Microsoft 365 eliminados para ser restaurado e clique em **restaurar o grupo**.</span><span class="sxs-lookup"><span data-stu-id="c635d-106">Select the deleted Microsoft 365 group/Teams to be restored and click **restore group**.</span></span>

    <span data-ttu-id="c635d-107">Se o grupo não puder ser restaurado por causa de um endereço SMTP conflituoso, use o seguinte comando para encontrar o objeto que está a causar conflito e remover o endereço SMTP:</span><span class="sxs-lookup"><span data-stu-id="c635d-107">If the group can't be restored because of a conflicting SMTP address, use following command to find the object that’s causing conflict and remove the SMTP address:</span></span>

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    <span data-ttu-id="c635d-108">**Nota:** Em alguns casos, pode levar até 24 horas para o grupo e todos os seus dados serem restaurados.</span><span class="sxs-lookup"><span data-stu-id="c635d-108">**Note:** In some cases, it might take as long as 24 hours for the group and all of its data to be restored.</span></span>

    <span data-ttu-id="c635d-109">Para obter mais informações ou para aprender a restaurar grupos usando o PowerShell, consulte [Restaurar um grupo Microsoft 365 eliminado](https://go.microsoft.com/fwlink/?linkid=867802).</span><span class="sxs-lookup"><span data-stu-id="c635d-109">For more info, or to learn how to restore groups using PowerShell, see [Restore a deleted Microsoft 365 group](https://go.microsoft.com/fwlink/?linkid=867802).</span></span>