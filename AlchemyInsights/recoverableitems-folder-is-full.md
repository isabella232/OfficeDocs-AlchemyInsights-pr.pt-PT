---
title: 1336 Pasta RecoveryAbleItems está cheia
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: fb10b792981040bdcf4661b8aff30733c2438212
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720263"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="4e42d-102">A pasta de Itens Recuperáveis está cheia</span><span class="sxs-lookup"><span data-stu-id="4e42d-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="4e42d-103">Para trocar caixas de correio online, o limite de armazenamento predefinido para a pasta "Itens Recuperáveis" é de 30 GB.</span><span class="sxs-lookup"><span data-stu-id="4e42d-103">For Exchange Online mailboxes, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="4e42d-104">O limite de armazenamento da pasta Itens Recuperáveis é automaticamente aumentado para 100 GB se a caixa de correio for colocada em Litigation Hold, eDiscovery hold ou for atribuída a uma política de retenção.</span><span class="sxs-lookup"><span data-stu-id="4e42d-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to a retention policy.</span></span>

<span data-ttu-id="4e42d-105">Quando a pasta "Itens Recuperáveis" atinge o limite de armazenamento, a funcionalidade da caixa de correio é afetada das seguintes formas:</span><span class="sxs-lookup"><span data-stu-id="4e42d-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="4e42d-106">O utilizador não pode apagar artigos da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="4e42d-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="4e42d-107">O Assistente de Pasta Gerida não pode eliminar itens com base na etiqueta de retenção ou nas definições de pasta geridas.</span><span class="sxs-lookup"><span data-stu-id="4e42d-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="4e42d-108">Para caixas de correio que tenham a Recuperação do Item Único ativada ou colocadas em espera, o processo de proteção da página copy-on-write não pode manter versões de itens editados pelo utilizador.</span><span class="sxs-lookup"><span data-stu-id="4e42d-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="4e42d-109">Para caixas de correio que tenham registo de auditoria de caixa de correio ativado, nenhuma entrada de registo de auditoria de caixa de correio pode ser guardada na subpasta de Auditorias na pasta Itens Recuperáveis.</span><span class="sxs-lookup"><span data-stu-id="4e42d-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="4e42d-110">Para caixas de correio que não estejam em espera, os administradores podem usar o `Search-Mailbox -SearchDumpsterOnly -DeleteContent` comando no Exchange Online PowerShell para eliminar itens na pasta Itens Recuperáveis.</span><span class="sxs-lookup"><span data-stu-id="4e42d-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="4e42d-111">For more information, see the following topics:</span><span class="sxs-lookup"><span data-stu-id="4e42d-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="4e42d-112">Pesquisar e eliminar mensagens</span><span class="sxs-lookup"><span data-stu-id="4e42d-112">Search for and delete messages</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="4e42d-113">Caixa de pesquisa-correio</span><span class="sxs-lookup"><span data-stu-id="4e42d-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="4e42d-114">Para as caixas de correio que estão em espera, os administradores têm de remover o porão antes de poderem apagar itens da pasta Itens Recuperáveis.</span><span class="sxs-lookup"><span data-stu-id="4e42d-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="4e42d-115">Para mais informações, consulte Apagar itens na pasta de [Itens Recuperáveis das caixas de correio baseadas na nuvem em espera](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="4e42d-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="4e42d-116">Para ajudar a evitar que a pasta De Itens Recuperáveis fique cheia, os administradores podem aumentar o limite de armazenamento da pasta De Itens Recuperáveis para caixas de correio em espera e configurar uma política de retenção de caixas de correio que transfere itens da pasta De Itens Recuperáveis para a caixa de correio de arquivo do utilizador.</span><span class="sxs-lookup"><span data-stu-id="4e42d-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="4e42d-117">Ver Aumentar a quota de [itens recuperáveis para caixas de correio em espera](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="4e42d-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
