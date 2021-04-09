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
# <a name="restore-a-deleted-microsoft-365-group"></a>Restaurar um grupo Microsoft 365 eliminado

Pode restaurar um grupo Microsoft 365 ou Microsoft Teams eliminados no prazo de 30 dias a partir da eliminação.

1. Vá ao [centro de administração microsoft 365](https://aka.ms/RestoreDeletedGroup) para iniciar sessão numa lista de vocês são os grupos e equipas eliminados.

    **Nota:** Faça login usando a conta que é atribuída ao administrador do inquilino ou à função de administrador de grupos.

1. Selecione o grupo/equipas do Microsoft 365 eliminados para ser restaurado e clique em **restaurar o grupo**.

    Se o grupo não puder ser restaurado por causa de um endereço SMTP conflituoso, use o seguinte comando para encontrar o objeto que está a causar conflito e remover o endereço SMTP:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Nota:** Em alguns casos, pode levar até 24 horas para o grupo e todos os seus dados serem restaurados.

    Para obter mais informações ou para aprender a restaurar grupos usando o PowerShell, consulte [Restaurar um grupo Microsoft 365 eliminado](https://go.microsoft.com/fwlink/?linkid=867802).