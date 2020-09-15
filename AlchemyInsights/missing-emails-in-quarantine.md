---
title: E-mails desaparecidos em quarentena
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 55ed9a92675939c05477fbf6d12bbedd6eb931d6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673725"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="2e13a-102">Faltando e-mails em quarentena"</span><span class="sxs-lookup"><span data-stu-id="2e13a-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="2e13a-103">Os administradores podem [ver, libertar ou eliminar estas mensagens.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="2e13a-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="2e13a-104">Para abrir o Centro de Conformidade & de Segurança, vá a [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="2e13a-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="2e13a-105">Para abrir a página de Quarentena diretamente, vá a [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="2e13a-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="2e13a-106">Pode pesquisar pelos seguintes valores:</span><span class="sxs-lookup"><span data-stu-id="2e13a-106">You can search by the following values:</span></span>  

- <span data-ttu-id="2e13a-107">**ID de mensagem**: O identificador globalmente único da mensagem.</span><span class="sxs-lookup"><span data-stu-id="2e13a-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="2e13a-108">Se selecionar uma mensagem na lista, o valor  **do ID**  da mensagem aparece no painel de voo  **de detalhes**  que aparece.</span><span class="sxs-lookup"><span data-stu-id="2e13a-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="2e13a-109">Os administradores podem usar [o rastreio de mensagens](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) para encontrar mensagens e os valores correspondentes do ID da mensagem.</span><span class="sxs-lookup"><span data-stu-id="2e13a-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="2e13a-110">**Endereço de e-mail remetente**: O endereço de e-mail de um único remetente.</span><span class="sxs-lookup"><span data-stu-id="2e13a-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="2e13a-111">**Endereço de e-mail do destinatário**: O endereço de e-mail de um único destinatário.</span><span class="sxs-lookup"><span data-stu-id="2e13a-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="2e13a-112">**Objeto**: Utilize todo o assunto da mensagem.</span><span class="sxs-lookup"><span data-stu-id="2e13a-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="2e13a-113">A procura não é sensível a casos.</span><span class="sxs-lookup"><span data-stu-id="2e13a-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="2e13a-114">Depois de introduzir os critérios de pesquisa, clique no ![ botão ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** para filtrar os resultados.  </span><span class="sxs-lookup"><span data-stu-id="2e13a-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="2e13a-115">Os cmdlets que usa para visualizar e gere mensagens e ficheiros em quarentena são:</span><span class="sxs-lookup"><span data-stu-id="2e13a-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="2e13a-116">Eliminar-QuarentenaMessage</span><span class="sxs-lookup"><span data-stu-id="2e13a-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="2e13a-117">Exportação-Quarentena</span><span class="sxs-lookup"><span data-stu-id="2e13a-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="2e13a-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="2e13a-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="2e13a-119">[Pré-visualização-QuarentenaMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note que este cmdlet é apenas para mensagens, não ficheiros de malware de ATP para SharePoint Online, OneDrive para Negócios ou Equipas.</span><span class="sxs-lookup"><span data-stu-id="2e13a-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="2e13a-120">Libertação-QuarentenaMessage</span><span class="sxs-lookup"><span data-stu-id="2e13a-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)