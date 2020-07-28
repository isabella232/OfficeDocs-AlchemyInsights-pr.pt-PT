---
title: Vários objetos têm o mesmo endereço de e-mail que identidade
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: cc932aa7ecbd1e338c409a7a6525e2c4e673b232
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439714"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a><span data-ttu-id="72e74-102">Vários objetos têm o mesmo endereço de e-mail que identidade</span><span class="sxs-lookup"><span data-stu-id="72e74-102">Multiple objects have the same email address as identity</span></span>

<span data-ttu-id="72e74-103">**Objetos múltiplos**</span><span class="sxs-lookup"><span data-stu-id="72e74-103">**Multiple objects**</span></span>

<span data-ttu-id="72e74-104">Uma das razões comuns deste erro é não ser capaz de encaminhar um pedido do Outlook Web Access corretamente na presença de vários objetos com o mesmo endereço de e-mail que a identidade.</span><span class="sxs-lookup"><span data-stu-id="72e74-104">One of the common reasons of this error is not being able to route an Outlook Web Access request properly in a presence of multiple objects having the same email address as identity.</span></span> <span data-ttu-id="72e74-105">Para encontrar estes objetos, executar os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="72e74-105">To find these objects, run the following commands:</span></span>

<span data-ttu-id="72e74-106">· Get-Recipient<email address></span><span class="sxs-lookup"><span data-stu-id="72e74-106">· Get-Recipient <email address></span></span>

<span data-ttu-id="72e74-107">· Get-User<email address></span><span class="sxs-lookup"><span data-stu-id="72e74-107">· Get-User <email address></span></span>

<span data-ttu-id="72e74-108">· Get-User <email address> -SoftDeletedUser</span><span class="sxs-lookup"><span data-stu-id="72e74-108">· Get-User <email address> -SoftDeletedUser</span></span>

<span data-ttu-id="72e74-109">· Obter Contacto<email address></span><span class="sxs-lookup"><span data-stu-id="72e74-109">· Get-Contact <email address></span></span>

<span data-ttu-id="72e74-110">· Get-Mailbox <email address> -PublicFolder</span><span class="sxs-lookup"><span data-stu-id="72e74-110">· Get-Mailbox <email address> -PublicFolder</span></span>

<span data-ttu-id="72e74-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span><span class="sxs-lookup"><span data-stu-id="72e74-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span></span>

<span data-ttu-id="72e74-112">· Get-Mailbox <email address> -InactiveMailboxOnly</span><span class="sxs-lookup"><span data-stu-id="72e74-112">· Get-Mailbox <email address> -InactiveMailboxOnly</span></span>

<span data-ttu-id="72e74-113">Para resolver o problema, remova vários objetos com a mesma identidade de e-mail e certifique-se de que existe um único objeto com a identidade específica do e-mail e que o seu tipo de destinatário é userMailbox.</span><span class="sxs-lookup"><span data-stu-id="72e74-113">To resolve the issue, remove multiple objects with the same email identity and make sure that there is a single object with the specific email identity and that its recipient type is UserMailbox.</span></span>

<span data-ttu-id="72e74-114">**O mesmo endereço é usado para caixas de correio de negócios e consumidores**</span><span class="sxs-lookup"><span data-stu-id="72e74-114">**Same address is used for business and consumer mailboxes**</span></span>

<span data-ttu-id="72e74-115">Outra das causas é quando o mesmo endereço é usado para caixas de correio de empresas e consumidores.</span><span class="sxs-lookup"><span data-stu-id="72e74-115">Another cause is when the same address is used for business and consumer mailboxes.</span></span> <span data-ttu-id="72e74-116">Neste caso, o utilizador deve alterar o seu pseudónimo principal de consumidor até que o Café suporte este cenário.</span><span class="sxs-lookup"><span data-stu-id="72e74-116">In this case, the user must change their primary consumer alias until Cafe supports this scenario.</span></span> <span data-ttu-id="72e74-117">Trata-se de um erro permanente que não desaparece sem intervenção.</span><span class="sxs-lookup"><span data-stu-id="72e74-117">This is a permanent error that does not go away without intervention.</span></span>

<span data-ttu-id="72e74-118">Para mais informações, consulte [alterar o endereço de e-mail ou o número de telefone da sua conta Microsoft.](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account)</span><span class="sxs-lookup"><span data-stu-id="72e74-118">For details, see [Change the email address or phone number for your Microsoft account](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span></span>