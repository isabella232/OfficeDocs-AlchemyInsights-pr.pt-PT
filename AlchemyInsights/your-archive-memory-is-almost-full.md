---
title: A sua caixa de correio de arquivo está quase cheia
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100006"
- "7960"
ms.openlocfilehash: 085d9b211d5a8e9a0e1eb12af14d87a4e59c844a3afa012095dfd60db316ad14
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046763"
---
# <a name="your-archive-mailbox-is-almost-full"></a>A sua caixa de correio de arquivo está quase cheia

Se o utilizador receber o aviso; **A sua caixa de correio de arquivo** está quase cheia ou tem de aumentar o tamanho da respetiva caixa de correio de arquivo. Eis algumas sugestões:

1. Se lhe for atribuída uma licença do Exchange Online 1, atualize para uma licença do **Exchange Online Plano 2** para aumentar o tamanho de 50 GB para 100 GB.
1. Se o utilizador já tiver atribuído uma das seguintes funcionalidades: Exchange Online Plano **2** ou um plano Exchange Online (Plano 1) com um adicionar Arquivo de Exchange Online, utilize os passos abaixo para ativar o arquivo de Expansão Automática:
 
    1. [Ligação a Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).
    2. Execute o seguinte comando para o utilizador:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. Execute o seguinte comando para confirmar que está ativado para o utilizador:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

Para obter mais informações, consulte:

- [Ativar o arquivo ilimitado – Ajuda para Administradores – Microsoft 365 em conformidade | Documentos da Microsoft](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Exchange Online - Descrições de Serviço | Documentos da Microsoft](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [Atualizar para um plano de negócios | Documentos da Microsoft](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

