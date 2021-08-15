---
title: E-mails em falta na quarentena
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
ms.openlocfilehash: 900d5f250846e9a7046f72156c150f4970d91d5ad94cb7fc054952228f4bf257
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54026233"
---
# <a name="missing-emails-in-quarantine"></a>E-mails em falta na quarentena"

Os [administradores podem ver, libertar ou eliminar estas mensagens.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

Para abrir o Centro de & de Conformidade, vá para [https://protection.office.com](https://protection.office.com/) . Para abrir a página quarentena diretamente, vá para [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Pode procurar pelos seguintes valores:  

- **ID da Mensagem:** o identificador exclusivo global da mensagem. Se selecionar uma mensagem na lista, o  **valor ID**  da Mensagem é apresentado no  **painel**  de lista de listas Detalhes que é apresentado. Os administradores podem utilizar o [rastreio de](/microsoft-365/security/office-365-security/message-trace-scc) mensagens para localizar mensagens e os respetivos valores de ID da Mensagem.
- **Endereço de e-mail do** remetente: o endereço de e-mail de um único remetente.
- **Endereço de e-mail do** destinatário: o endereço de e-mail de um único destinatário.
- **Assunto:** Utilize o assunto completo da mensagem. A pesquisa não é sensível a casos sensíveis às mesmas.

Após ter introduzido os critérios de pesquisa, clique no botão ![ ](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Atualizar, atualizar** para filtrar os resultados.

Os cmdlets que utiliza para ver e gerir mensagens e ficheiros na quarentena são:
- [Delete-QuarantineMessage](/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage](/powershell/module/exchange/preview-quarantinemessage): tenha em atenção que este cmdlet é apenas para mensagens e não para ficheiros malware do Microsoft Defender para Office 365 para SharePoint Online, OneDrive para Empresas ou Teams.
- [Release-QuarantineMessage](/powershell/module/exchange/release-quarantinemessage)