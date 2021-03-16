---
title: Remova o serviço de fundo para a Pesquisa do Microsoft em Bing
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816334"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a><span data-ttu-id="9f241-102">Remova o serviço de fundo para a Pesquisa do Microsoft em Bing</span><span class="sxs-lookup"><span data-stu-id="9f241-102">Remove the background service for Microsoft Search in Bing</span></span>

<span data-ttu-id="9f241-103">Para remover o serviço de fundo para a Pesquisa do Microsoft em Bing, pode experimentar os seguintes remédios:</span><span class="sxs-lookup"><span data-stu-id="9f241-103">To remove the background service for Microsoft Search in Bing, you can try the following remedies:</span></span>

1. <span data-ttu-id="9f241-104">Para reverter para as definições originais do motor de busca, faça as seguintes coisas:</span><span class="sxs-lookup"><span data-stu-id="9f241-104">To revert to the original search engine settings, do the following things:</span></span>

    <span data-ttu-id="9f241-105">a.</span><span class="sxs-lookup"><span data-stu-id="9f241-105">a.</span></span> <span data-ttu-id="9f241-106">Mude o **Use Bing como o seu motor de busca predefinido [para desligar](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome)**.</span><span class="sxs-lookup"><span data-stu-id="9f241-106">Switch the **Use Bing as your default search engine [toggle](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) Off**.</span></span>

    <span data-ttu-id="9f241-107">b.</span><span class="sxs-lookup"><span data-stu-id="9f241-107">b.</span></span> <span data-ttu-id="9f241-108">[Vá ao centro de administração microsoft 365](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) e limpe a definição que afeta todos os utilizadores da sua organização.</span><span class="sxs-lookup"><span data-stu-id="9f241-108">[Go to the Microsoft 365 admin center](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) and clear the setting that affects all users in your organization.</span></span>

2. <span data-ttu-id="9f241-109">Para remover o serviço de fundo de um dispositivo individual, faça as seguintes tarefas:</span><span class="sxs-lookup"><span data-stu-id="9f241-109">To remove the background service from an individual device, do the following tasks:</span></span>

    <span data-ttu-id="9f241-110">a.</span><span class="sxs-lookup"><span data-stu-id="9f241-110">a.</span></span> <span data-ttu-id="9f241-111">Escolha **o Painel de Controlo > programas > programas e funcionalidades**.</span><span class="sxs-lookup"><span data-stu-id="9f241-111">Choose **Control Panel > Programs > Programs and Features**.</span></span>

    <span data-ttu-id="9f241-112">b.</span><span class="sxs-lookup"><span data-stu-id="9f241-112">b.</span></span> <span data-ttu-id="9f241-113">Clique com o botão direito **Google in Bing** na lista de programas instalados e, em seguida, clique em **Desinstalar**.</span><span class="sxs-lookup"><span data-stu-id="9f241-113">Right-click **Microsoft Search in Bing** under the list of installed programs, and then click **Uninstall**.</span></span>

3. <span data-ttu-id="9f241-114">Para remover o serviço de fundo de vários dispositivos na sua organização, faça login como administrador e execute o seguinte comando num script:</span><span class="sxs-lookup"><span data-stu-id="9f241-114">To remove the background service from multiple devices in your organization, log in as an administrator and run the following command in a script:</span></span> 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
