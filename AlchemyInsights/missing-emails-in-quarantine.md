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
ms.openlocfilehash: 563f76f624f428a46894268b478cf05eb757b497
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539835"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="86265-102">E-mails em falta na quarentena"</span><span class="sxs-lookup"><span data-stu-id="86265-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="86265-103">Os [administradores podem ver, libertar ou eliminar estas mensagens.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)</span><span class="sxs-lookup"><span data-stu-id="86265-103">Administrators can [view, release, or delete these messages.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)</span></span>

<span data-ttu-id="86265-104">Para abrir o Centro de & de Conformidade, vá para [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="86265-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="86265-105">Para abrir a página quarentena diretamente, vá para [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="86265-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="86265-106">Pode procurar pelos seguintes valores:</span><span class="sxs-lookup"><span data-stu-id="86265-106">You can search by the following values:</span></span>  

- <span data-ttu-id="86265-107">**ID da Mensagem:** o identificador exclusivo global da mensagem.</span><span class="sxs-lookup"><span data-stu-id="86265-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="86265-108">Se selecionar uma mensagem na lista, o  **valor ID**  da Mensagem é apresentado no  **painel**  de lista de listas Detalhes que é apresentado.</span><span class="sxs-lookup"><span data-stu-id="86265-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="86265-109">Os administradores podem utilizar o [rastreio de](/microsoft-365/security/office-365-security/message-trace-scc) mensagens para localizar mensagens e os respetivos valores de ID da Mensagem.</span><span class="sxs-lookup"><span data-stu-id="86265-109">Admins can use [message trace](/microsoft-365/security/office-365-security/message-trace-scc) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="86265-110">**Endereço de e-mail do** remetente: o endereço de e-mail de um único remetente.</span><span class="sxs-lookup"><span data-stu-id="86265-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="86265-111">**Endereço de e-mail do** destinatário: o endereço de e-mail de um único destinatário.</span><span class="sxs-lookup"><span data-stu-id="86265-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="86265-112">**Assunto:** Utilize o assunto completo da mensagem.</span><span class="sxs-lookup"><span data-stu-id="86265-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="86265-113">A pesquisa não é sensível a casos sensíveis às mesmas.</span><span class="sxs-lookup"><span data-stu-id="86265-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="86265-114">Após ter introduzido os critérios de pesquisa, clique no botão ![ ](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Atualizar, atualizar** para filtrar os resultados.</span><span class="sxs-lookup"><span data-stu-id="86265-114">After you've entered the search criteria, click ![Refresh button](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** to filter the results.</span></span>

<span data-ttu-id="86265-115">Os cmdlets que utiliza para ver e gerir mensagens e ficheiros na quarentena são:</span><span class="sxs-lookup"><span data-stu-id="86265-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="86265-116">Delete-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="86265-116">Delete-QuarantineMessage</span></span>](/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="86265-117">Export-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="86265-117">Export-QuarantineMessage</span></span>](/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="86265-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="86265-118">Get-QuarantineMessage</span></span>](/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="86265-119">[Preview-QuarantineMessage](/powershell/module/exchange/preview-quarantinemessage): tenha em atenção que este cmdlet é apenas para mensagens e não para ficheiros malware do Microsoft Defender para Office 365 para SharePoint Online, OneDrive para Empresas ou Teams.</span><span class="sxs-lookup"><span data-stu-id="86265-119">[Preview-QuarantineMessage](/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from Microsoft Defender for Office 365 for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="86265-120">Release-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="86265-120">Release-QuarantineMessage</span></span>](/powershell/module/exchange/release-quarantinemessage)