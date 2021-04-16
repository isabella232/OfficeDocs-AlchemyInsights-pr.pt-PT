---
title: Clicar duas vezes num ficheiro do Office não consegue abri-lo
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
- "2200002"
- "161"
ms.openlocfilehash: b9c563f7dd099bf3bad9018f69e2096816dd7290
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814816"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a><span data-ttu-id="bebe5-102">Clicar duas vezes num ficheiro do Office não consegue abri-lo</span><span class="sxs-lookup"><span data-stu-id="bebe5-102">Double-clicking an Office file fails to open it</span></span>

<span data-ttu-id="bebe5-103">Depois de clicar duas vezes num ficheiro do Office, pode ver o programa aberto, mas o ficheiro em si não abre.</span><span class="sxs-lookup"><span data-stu-id="bebe5-103">After double-clicking an Office file, you may see the program open but the file itself doesn't open.</span></span> <span data-ttu-id="bebe5-104">Ou pode ter o erro: "Houve um problema em enviar o comando para o programa."</span><span class="sxs-lookup"><span data-stu-id="bebe5-104">Or you may get the error: "There was a problem sending the command to the program."</span></span> <span data-ttu-id="bebe5-105">Há muitas causas para isso, mas as duas soluções mais comuns são:</span><span class="sxs-lookup"><span data-stu-id="bebe5-105">There are many causes for this, but the two most common solutions are:</span></span>

- <span data-ttu-id="bebe5-106">A partir do Excel, certifique-se de que a opção DDE não está controlada.</span><span class="sxs-lookup"><span data-stu-id="bebe5-106">From within Excel, ensure that the DDE option is unchecked.</span></span> <span data-ttu-id="bebe5-107">A opção pode ser encontrada criando um novo livro de trabalho e, em seguida, escolhendo **Opções de > de Arquivo > Advanced**.</span><span class="sxs-lookup"><span data-stu-id="bebe5-107">The option can be found by creating a new workbook and then choosing **File > Options > Advanced**.</span></span> <span data-ttu-id="bebe5-108">Na secção **Geral,** desmarque as **outras aplicações que utilizam a Dynamic Data Exchange (DDE)**.</span><span class="sxs-lookup"><span data-stu-id="bebe5-108">In the **General** section, uncheck the **Ignore other applications that use Dynamic Data Exchange (DDE)**.</span></span>

- <span data-ttu-id="bebe5-109">Executar uma Reparação On-line para restaurar as definições predefinidos.</span><span class="sxs-lookup"><span data-stu-id="bebe5-109">Run an Online Repair to restore default settings.</span></span> <span data-ttu-id="bebe5-110">Clique no botão Iniciar o Windows e procure "Painel de Controlo".</span><span class="sxs-lookup"><span data-stu-id="bebe5-110">Click the Windows Start button and search for "Control Panel."</span></span> <span data-ttu-id="bebe5-111">Abra o **Painel de Controlo** e vá a Programas > Programas e **Funcionalidades**.</span><span class="sxs-lookup"><span data-stu-id="bebe5-111">Open the **Control Panel**, and go to **Programs > Programs and Features**.</span></span> <span data-ttu-id="bebe5-112">Em seguida, clique com o botão direito **microsoft Office [versão]** e escolha **Change > Online Repair**.</span><span class="sxs-lookup"><span data-stu-id="bebe5-112">Then right-click **Microsoft Office [Version]** and choose **Change > Online Repair**.</span></span>

<span data-ttu-id="bebe5-113">Se nenhuma destas soluções funcionar, uma lista mais completa de soluções pode ser encontrada no artigo de suporte, [clicando duas vezes num ficheiro do Office não o abre](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span><span class="sxs-lookup"><span data-stu-id="bebe5-113">If neither of these solutions work, a more complete list of solutions can be found in the support article, [Double-clicking an Office file fails to open it](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span></span>
