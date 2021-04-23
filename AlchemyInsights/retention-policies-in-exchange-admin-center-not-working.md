---
title: As Políticas de Retenção no Centro de Administração do Exchange não funcionam
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: bb2ce7ce2405be575dfdb79d304fef690e863a4e
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952239"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="01669-102">Políticas de Retenção no Centro de Administração do Exchange</span><span class="sxs-lookup"><span data-stu-id="01669-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="01669-103">Se quiser que executemos verificações automáticas das definições mencionadas abaixo, selecione o botão Back < -- na parte superior desta página e, em seguida, introduza o endereço de e-mail do utilizador que tem problemas com as políticas de retenção.</span><span class="sxs-lookup"><span data-stu-id="01669-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

<span data-ttu-id="01669-104">Se tiver problemas com as políticas de retenção no Centro de Administração do Exchange que não se aplicam a caixas de correio ou itens que não estão a ser movidos para a caixa de correio de arquivo, verifique o seguinte:</span><span class="sxs-lookup"><span data-stu-id="01669-104">If you have problems with retention policies in the Exchange Admin Center not applying to mailboxes or items not moving to the archive mailbox, check the following:</span></span>

<span data-ttu-id="01669-105">**Causas Raiz:**</span><span class="sxs-lookup"><span data-stu-id="01669-105">**Root Causes:**</span></span>

- <span data-ttu-id="01669-106">**O Assistente de Pastas** Geridas não processou a caixa de correio do utilizador.</span><span class="sxs-lookup"><span data-stu-id="01669-106">**Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="01669-107">O Assistente de Pastas Geridas tenta processar todas as caixas de correio na sua organização baseada na nuvem uma vez a cada sete dias.</span><span class="sxs-lookup"><span data-stu-id="01669-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span>

  <span data-ttu-id="01669-108">**Solução:** Execute o Assistente de Pastas Geridas.</span><span class="sxs-lookup"><span data-stu-id="01669-108">**Solution:** Run the Managed Folder Assistant.</span></span>

- <span data-ttu-id="01669-109">**O RetentionHold** foi **ativado** na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="01669-109">**RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="01669-110">Se a caixa de correio tiver sido colocada num RetentionHold, a política de retenção na caixa de correio não será processada durante esse período de tempo.</span><span class="sxs-lookup"><span data-stu-id="01669-110">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span>

  <span data-ttu-id="01669-111">**Solução:** Verifique o estado da definição e atualização da Retenção conforme necessário.</span><span class="sxs-lookup"><span data-stu-id="01669-111">**Solution:** Check status of Retention Hold setting and update as needed.</span></span> <span data-ttu-id="01669-112">Para obter detalhes, consulte [o artigo Retenção na Caixa de Correio](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="01669-112">For details, see [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
 
<span data-ttu-id="01669-113">**Nota:** Se uma caixa de correio for inferior a 10 MB, o Assistente de Pastas Geridas não processará automaticamente a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="01669-113">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="01669-114">Para mais informações sobre políticas de retenção no Centro de Administração do Exchange, consulte:</span><span class="sxs-lookup"><span data-stu-id="01669-114">For more info on retention policies in the Exchange Admin Center, see:</span></span>

- [<span data-ttu-id="01669-115">Etiquetas de retenção e políticas de retenção</span><span class="sxs-lookup"><span data-stu-id="01669-115">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- <span data-ttu-id="01669-116">[Aplicar uma política de retenção a caixas de correio](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) ou [Adicionar ou remover etiquetas de retenção](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span><span class="sxs-lookup"><span data-stu-id="01669-116">[Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) or [Add or remove retention tags](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span></span>

- [<span data-ttu-id="01669-117">Como identificar o tipo de reter colocado numa caixa de correio</span><span class="sxs-lookup"><span data-stu-id="01669-117">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
