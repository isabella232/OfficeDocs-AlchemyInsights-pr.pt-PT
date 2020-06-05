---
title: E-mails desaparecidos em quarentena
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 61a926c363c62bc7acb5efefe42b834f33c78eb6
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569556"
---
# <a name="missing-emails-in-quarantine"></a>Faltando e-mails em quarentena"

Os administradores podem [ver, libertar ou eliminar estas mensagens.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Para abrir o Centro de Conformidade & de Segurança, vá a [https://protection.office.com](https://protection.office.com/) . Para abrir a página de Quarentena diretamente, vá a [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Pode pesquisar pelos seguintes valores:  

- **ID de mensagem**: O identificador globalmente único da mensagem. Se selecionar uma mensagem na lista, o valor **do ID** da mensagem aparece no painel de voo **de detalhes** que aparece. Os administradores podem usar [o rastreio de mensagens](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) para encontrar mensagens e os valores correspondentes do ID da mensagem.
- **Endereço de e-mail remetente**: O endereço de e-mail de um único remetente.
- **Endereço de e-mail do destinatário**: O endereço de e-mail de um único destinatário.
- **Objeto**: Utilize todo o assunto da mensagem. A procura não é sensível a casos.

Depois de introduzir os critérios de pesquisa, clique no ![ botão ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** para filtrar os resultados.  

Os cmdlets que usa para visualizar e gere mensagens e ficheiros em quarentena são:
- [Eliminar-QuarentenaMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Exportação-Quarentena](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Pré-visualização-QuarentenaMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note que este cmdlet é apenas para mensagens, não ficheiros de malware de ATP para SharePoint Online, OneDrive para Negócios ou Equipas.
- [Libertação-QuarentenaMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)