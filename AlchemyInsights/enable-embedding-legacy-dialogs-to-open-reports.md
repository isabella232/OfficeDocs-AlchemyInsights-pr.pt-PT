---
title: Ativar caixas de diálogo incorporadas para abrir relatórios
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: c8a5634d5d79cbd584284b675e5db4e448a0d157
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814275"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a><span data-ttu-id="28cc2-102">Ativar caixas de diálogo incorporadas para abrir relatórios</span><span class="sxs-lookup"><span data-stu-id="28cc2-102">Enable embedding legacy dialogs to open reports</span></span>

<span data-ttu-id="28cc2-103">**Sintoma**</span><span class="sxs-lookup"><span data-stu-id="28cc2-103">**Symptom**</span></span>

<span data-ttu-id="28cc2-104">Os utilizadores não conseguem abrir relatórios.</span><span class="sxs-lookup"><span data-stu-id="28cc2-104">Users are unable to open reports.</span></span> <span data-ttu-id="28cc2-105">"Algo correu mal.</span><span class="sxs-lookup"><span data-stu-id="28cc2-105">"Something has gone wrong.</span></span> <span data-ttu-id="28cc2-106">Consulte os detalhes técnicos para obter mais detalhes. "</span><span class="sxs-lookup"><span data-stu-id="28cc2-106">Check technical details for more details."</span></span>

<span data-ttu-id="28cc2-107">**Causa**</span><span class="sxs-lookup"><span data-stu-id="28cc2-107">**Cause**</span></span>

<span data-ttu-id="28cc2-108">Os relatórios não estão a carregar o UCI com o erro "o descritor de formulários é nulo ou não está definido".</span><span class="sxs-lookup"><span data-stu-id="28cc2-108">Reports are failing to load in UCI with the error, "Form descriptor is null or not defined."</span></span> <span data-ttu-id="28cc2-109">Os relatórios no UCI ainda requerem caixas de diálogo legadas, por isso, o sistema do cliente precisa de ter *allowlegacydialogsembedding* ativadas.</span><span class="sxs-lookup"><span data-stu-id="28cc2-109">Reports in UCI still require legacy dialogs, so the customer's system needs to have *allowlegacydialogsembedding* enabled.</span></span>

<span data-ttu-id="28cc2-110">**Solução**</span><span class="sxs-lookup"><span data-stu-id="28cc2-110">**Solution**</span></span>

1. <span data-ttu-id="28cc2-111">Aceda a **Definições > Administração > Definições do sistema > Separador Geral**.</span><span class="sxs-lookup"><span data-stu-id="28cc2-111">Go to **Settings >Administration > System Settings > General tab**.</span></span>

2. <span data-ttu-id="28cc2-112">Defina "Ativar a incorporação de determinadas caixas de diálogo legadas no cliente do browser da interface unificada" para **Sim**.</span><span class="sxs-lookup"><span data-stu-id="28cc2-112">Set "Enable embedding of certain legacy dialogs in Unified Interface browser client" to **Yes**.</span></span>
