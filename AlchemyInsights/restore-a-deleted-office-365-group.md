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
# <a name="restore-a-deleted-microsoft-365-group"></a>Restaurar um grupo Microsoft 365 eliminado

Pode restaurar um grupo Microsoft 365 ou Microsoft Teams eliminados no prazo de 30 dias a partir da eliminação.

1. Vá ao [centro de administração microsoft 365](https://aka.ms/RestoreDeletedGroup) para iniciar sessão e listar os grupos e equipas eliminados.

    **Nota:** Faça login usando a conta que é atribuída ao administrador do inquilino ou à função de administrador de grupos.

1. Selecione o grupo/equipas do Microsoft 365 eliminados para ser restaurado e clique em **restaurar o grupo**.

    Se o grupo não puder ser restaurado por causa de um endereço SMTP conflituoso, use o seguinte comando para encontrar o objeto que está a causar conflito e remover o endereço SMTP:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Nota:** Em alguns casos, pode levar até 24 horas para o grupo e todos os seus dados serem restaurados.

    Para obter mais informações ou para aprender a restaurar grupos usando o PowerShell, consulte [Restaurar um grupo Microsoft 365 eliminado](https://go.microsoft.com/fwlink/?linkid=867802).