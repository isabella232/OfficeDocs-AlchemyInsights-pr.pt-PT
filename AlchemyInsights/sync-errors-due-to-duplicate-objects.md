---
title: 902 (erros de sincronização devido a objectos duplicados)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 777c2d8d530d03d58180f43b362ee065439b56b3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507426"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="7ef9d-102">Erros de sincronização devido a objectos duplicados</span><span class="sxs-lookup"><span data-stu-id="7ef9d-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="7ef9d-103">Poderá receber uma das seguintes mensagens de erro quando concluir a sincronização de directórios no Office 365:</span><span class="sxs-lookup"><span data-stu-id="7ef9d-103">You might receive one of the following error messages when directory synchronization finishes in Office 365:</span></span>

- <span data-ttu-id="7ef9d-104">Não é possível actualizar este objecto no Microsoft Online Services porque os seguintes atributos associados a este objecto tem valores que já esteja associados a outro objecto no directório local.</span><span class="sxs-lookup"><span data-stu-id="7ef9d-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="7ef9d-105">Já existe um objecto sincronizado com o mesmo endereço de proxy no directório do Microsoft Online Services.</span><span class="sxs-lookup"><span data-stu-id="7ef9d-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="7ef9d-106">Não é possível actualizar este objecto porque os seguintes atributos associados a este objecto tem valores que já esteja associados a outro objecto os serviços de directório local: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="7ef9d-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="7ef9d-107">Para identificar e corrigir o problema, transfira e execute a [Ferramenta de reparação do IdFix DirSync erros](https://www.microsoft.com/download/details.aspx?id=36832).</span><span class="sxs-lookup"><span data-stu-id="7ef9d-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>

<span data-ttu-id="7ef9d-108">Para mais informações, consulte [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="7ef9d-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
