---
title: Falha na resolução de problemas oneDrive
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
- "9003084"
- "5885"
ms.openlocfilehash: 4bf45e7780dcbabb95b3eecfb2df55beffde11d6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826210"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="ef3d4-102">Falha na resolução de problemas oneDrive</span><span class="sxs-lookup"><span data-stu-id="ef3d4-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="ef3d4-103">Se o OneDrive se despenhar repetidamente, experimente estes passos de resolução de problemas:</span><span class="sxs-lookup"><span data-stu-id="ef3d4-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="ef3d4-104">**Certifique-se de que as chaves de registo não estão definidas:**</span><span class="sxs-lookup"><span data-stu-id="ef3d4-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="ef3d4-105">Utilizando o Editor de Registos, navegue para HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="ef3d4-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="ef3d4-106">Se o DisableFileSyncNGSC estiver presente e definido para 1, abra a chave e altere o valor para 0.</span><span class="sxs-lookup"><span data-stu-id="ef3d4-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="ef3d4-107">Lançar manualmente o OneDrive indo para iniciar</span><span class="sxs-lookup"><span data-stu-id="ef3d4-107">Manually launch OneDrive by going to Start</span></span> ![Prima a tecla Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="ef3d4-109">, digite OneDrive na caixa de pesquisa e, em seguida, clique na aplicação de ambiente de trabalho OneDrive.</span><span class="sxs-lookup"><span data-stu-id="ef3d4-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="ef3d4-110">**Reset OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="ef3d4-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="ef3d4-111">Notas:</span><span class="sxs-lookup"><span data-stu-id="ef3d4-111">Notes:</span></span>

- <span data-ttu-id="ef3d4-112">A reposição do OneDrive desliga todas as suas ligações de sincronização existentes (incluindo o seu OneDrive pessoal se estiver configurado).</span><span class="sxs-lookup"><span data-stu-id="ef3d4-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="ef3d4-113">Não perderá ficheiros ou dados repondo o OneDrive no seu computador.</span><span class="sxs-lookup"><span data-stu-id="ef3d4-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="ef3d4-114">**Para redefinir o OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="ef3d4-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="ef3d4-115">Abra um diálogo executar premindo a tecla do Windows e R.</span><span class="sxs-lookup"><span data-stu-id="ef3d4-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="ef3d4-116">Digite %localappdata%\Microsoft\OneDrive\onedrive.exe /reset e prima OK.</span><span class="sxs-lookup"><span data-stu-id="ef3d4-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="ef3d4-117">Uma janela de comando pode aparecer brevemente.</span><span class="sxs-lookup"><span data-stu-id="ef3d4-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="ef3d4-118">Lançar manualmente o OneDrive indo para iniciar</span><span class="sxs-lookup"><span data-stu-id="ef3d4-118">Manually launch OneDrive by going to Start</span></span> ![Prima a tecla Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="ef3d4-120">, digite OneDrive na caixa de pesquisa e, em seguida, clique na aplicação de ambiente de trabalho OneDrive.</span><span class="sxs-lookup"><span data-stu-id="ef3d4-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="ef3d4-121">Notas:</span><span class="sxs-lookup"><span data-stu-id="ef3d4-121">Notes:</span></span>

- <span data-ttu-id="ef3d4-122">Se tivesse optado por sincronizar apenas algumas pastas antes do reset, terá de o fazer novamente uma vez concluída a sincronização.</span><span class="sxs-lookup"><span data-stu-id="ef3d4-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="ef3d4-123">Leia [Escolha quais as pastas OneDrive para sincronizar o computador](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)para obter mais   informações.</span><span class="sxs-lookup"><span data-stu-id="ef3d4-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="ef3d4-124">Terá de completar isto para o seu OneDrive pessoal e OneDrive para negócios.</span><span class="sxs-lookup"><span data-stu-id="ef3d4-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>