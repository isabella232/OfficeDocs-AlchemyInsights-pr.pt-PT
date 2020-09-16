---
title: O proprietário não pode criar sub-pasta usando o Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 9590f780cffeaf644733752c763e04d748b1b39e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665729"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="6bf2c-102">O proprietário não pode criar sub-pasta usando o Outlook</span><span class="sxs-lookup"><span data-stu-id="6bf2c-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="6bf2c-103">**Há um problema contínuo com os proprietários de pastas públicas que criam sub-dobradores usando o Outlook. A questão será resolvida em breve.**</span><span class="sxs-lookup"><span data-stu-id="6bf2c-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="6bf2c-104">Entretanto, utilize uma das seguintes soluções alternativas:</span><span class="sxs-lookup"><span data-stu-id="6bf2c-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="6bf2c-105">Use outlook para MAC para criar a sub-dobradeira, uma vez que o problema impacta apenas o Outlook para janelas de ambiente de trabalho (todas as versões)</span><span class="sxs-lookup"><span data-stu-id="6bf2c-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="6bf2c-106">Ter a administração criar a subpasta usando EXO Shell ou EAC</span><span class="sxs-lookup"><span data-stu-id="6bf2c-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="6bf2c-107">Altere a Caixa postal/Correio de Correio por defeitoPublicFoldermailbox no utilizador para outra caixa de correio que a caixa de correio de conteúdo para a pasta que causa problema</span><span class="sxs-lookup"><span data-stu-id="6bf2c-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="6bf2c-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="6bf2c-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="6bf2c-109">Espere por uma hora, reinicie o cliente outlook</span><span class="sxs-lookup"><span data-stu-id="6bf2c-109">Wait for an hour, restart outlook client</span></span>