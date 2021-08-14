---
title: Restaurar um grupo de Microsoft 365 eliminado
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
ms.openlocfilehash: 6262ca04335c355fb4de41a9e1d854b666f47e10321a843717d6eb951c46cafd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53959037"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Restaurar um grupo de Microsoft 365 eliminado

Pode restaurar um grupo de Microsoft 365 eliminado ou Microsoft Teams dentro de 30 dias a partir da eliminação.

1. Aceda à [centro de administração do Microsoft 365](https://aka.ms/RestoreDeletedGroup) para iniciar sessão numa lista de equipas e grupos eliminados.

    **Nota:** Indique sessão com a conta atribuída ao administrador inquilino ou à função de administrador de grupos.

1. Selecione o grupo Microsoft 365/Teams pretende ser restaurado e clique em **Restaurar grupo**.

    Se não for possível restaurar o grupo devido a um endereço SMTP em conflito, utilize o seguinte comando para encontrar o objeto que está a causar o conflito e remova o endereço SMTP:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Nota:** Em alguns casos, pode demorar até 24 horas para que o grupo e todos os seus dados sejam restaurados.

    Para mais informações ou para saber como restaurar grupos com o PowerShell, consulte Restaurar um [grupo de Microsoft 365 eliminado.](https://go.microsoft.com/fwlink/?linkid=867802)