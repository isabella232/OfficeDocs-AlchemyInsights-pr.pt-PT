---
title: E-mails desaparecidos em quarentena
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 43f9a1f03084bf9adab706b3f77eff1d1db888ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831745"
---
# <a name="missing-emails-in-quarantine"></a>Faltando e-mails em quarentena"

Os administradores podem [ver, libertar ou eliminar estas mensagens.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Para abrir o Centro de Conformidade & de Segurança, vá a [https://protection.office.com](https://protection.office.com/) . Para abrir a página de Quarentena diretamente, vá a [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Pode pesquisar pelos seguintes valores:  

- **ID de mensagem**: O identificador globalmente único da mensagem. Se selecionar uma mensagem na lista, o valor  **do ID**  da mensagem aparece no painel de voo  **de detalhes**  que aparece. Os administradores podem usar [o rastreio de mensagens](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) para encontrar mensagens e os valores correspondentes do ID da mensagem.
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