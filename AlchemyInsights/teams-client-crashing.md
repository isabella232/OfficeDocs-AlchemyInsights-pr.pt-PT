---
title: O cliente do Teams está a falhar?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ce37b260d126f876d2b6177515bd8a7c3874ef2c
ms.sourcegitcommit: d02e2b73aa7d0453d7baca1ea5a186cf6081d022
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/27/2020
ms.locfileid: "43030677"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="a6381-102">O cliente do Teams está a falhar?</span><span class="sxs-lookup"><span data-stu-id="a6381-102">Teams client crashing?</span></span>

<span data-ttu-id="a6381-103">Se o seu cliente do Teams estiver a falhar, tente o seguinte:</span><span class="sxs-lookup"><span data-stu-id="a6381-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="a6381-104">Se estiver a utilizar a aplicação de ambiente de trabalho do Teams, [certifique-se de que a aplicação está totalmente atualizada](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="a6381-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="a6381-105">Certifique-se de que todos os [URLs e intervalos de endereços do Office 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) estão acessíveis.</span><span class="sxs-lookup"><span data-stu-id="a6381-105">Make sure all the [Office 365 URL's and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="a6381-106">Inicie sessão com a sua conta de administração e verifique o seu [Dashboard do Estado de Funcionamento do Serviço](https://docs.microsoft.com/office365/enterprise/view-service-health) para verificar se não existe qualquer interrupção ou degradação do serviço.</span><span class="sxs-lookup"><span data-stu-id="a6381-106">Log in with your admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

 - <span data-ttu-id="a6381-107">Como último passo, pode tentar limpar a cache do seu cliente do Teams:</span><span class="sxs-lookup"><span data-stu-id="a6381-107">As a last step, you can attempt to clear your Teams client cache:</span></span>

    1.  <span data-ttu-id="a6381-108">Saia completamente do cliente de ambiente de trabalho do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="a6381-108">Fully exit the Microsoft Teams desktop client.</span></span> <span data-ttu-id="a6381-109">Pode clicar com o botão direito do rato em **Teams** na área do tabuleiro de sistema e clique em **Sair**, ou execute o Gestor de Tarefas e termine totalmente o processo.</span><span class="sxs-lookup"><span data-stu-id="a6381-109">You can right-click **Teams** from the Icon Tray and click **Quit**, or run Task Manager and fully kill the process.</span></span>

    2.  <span data-ttu-id="a6381-110">Aceda ao Explorador de Ficheiros e escreva %appdata%\Microsoft\teams.</span><span class="sxs-lookup"><span data-stu-id="a6381-110">Go to File Explorer, and type in %appdata%\Microsoft\teams.</span></span>

    3.  <span data-ttu-id="a6381-111">Uma vez no diretório, verá algumas das seguintes pastas:</span><span class="sxs-lookup"><span data-stu-id="a6381-111">Once in the directory, you'll see a few of the following folders:</span></span>

         - <span data-ttu-id="a6381-112">Em **Cache de Aplicação**, aceda a Cache e elimine qualquer um dos ficheiros na localização da Cache:  %appdata%\Microsoft\teams\application cache\cache.</span><span class="sxs-lookup"><span data-stu-id="a6381-112">From within **Application Cache**, go to Cache and delete any of the files in the Cache location:  %appdata%\Microsoft\teams\application cache\cache.</span></span>

        - <span data-ttu-id="a6381-113">Em **Blob_storage**, elimine todos os ficheiros: %appdata%\Microsoft\teams\blob_storage.</span><span class="sxs-lookup"><span data-stu-id="a6381-113">From within **Blob_storage**, delete all files: %appdata%\Microsoft\teams\blob_storage.</span></span>

        - <span data-ttu-id="a6381-114">Em **Cache**, elimine todos os ficheiros: %appdata%\Microsoft\teams\Cache.</span><span class="sxs-lookup"><span data-stu-id="a6381-114">From within **Cache**, delete all files: %appdata%\Microsoft\teams\Cache.</span></span>

        - <span data-ttu-id="a6381-115">Em **databases**, elimine todos os ficheiros: %appdata%\Microsoft\teams\databases.</span><span class="sxs-lookup"><span data-stu-id="a6381-115">From within **databases**, delete all files: %appdata%\Microsoft\teams\databases.</span></span>

        - <span data-ttu-id="a6381-116">Em **GPUCache**, elimine todos os ficheiros: %appdata%\Microsoft\teams\GPUcache.</span><span class="sxs-lookup"><span data-stu-id="a6381-116">From within **GPUCache**, delete all files: %appdata%\Microsoft\teams\GPUcache.</span></span>

        - <span data-ttu-id="a6381-117">Em **IndexedDB**, elimine o ficheiro .db: %appdata%\Microsoft\teams\IndexedDB.</span><span class="sxs-lookup"><span data-stu-id="a6381-117">From within **IndexedDB**, delete the .db file: %appdata%\Microsoft\teams\IndexedDB.</span></span>

        - <span data-ttu-id="a6381-118">Em **Local Storage**, elimine todos os ficheiros: %appdata%\Microsoft\teams\Local Storage.</span><span class="sxs-lookup"><span data-stu-id="a6381-118">From within **Local Storage**, delete all files: %appdata%\Microsoft\teams\Local Storage.</span></span>

        - <span data-ttu-id="a6381-119">Por último, em **tmp**, elimine qualquer ficheiro: %appdata%\Microsoft\teams\tmp.</span><span class="sxs-lookup"><span data-stu-id="a6381-119">Lastly, from within **tmp**, delete any file: %appdata%\Microsoft\teams\tmp.</span></span>

    4. <span data-ttu-id="a6381-120">Reinicie o seu cliente do Teams.</span><span class="sxs-lookup"><span data-stu-id="a6381-120">Restart your Teams client.</span></span>
