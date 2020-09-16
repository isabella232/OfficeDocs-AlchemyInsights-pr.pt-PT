---
title: Mitigar o erro A aplicação não foi detetada
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000171"
- "1712"
ms.openlocfilehash: 498c2ec78bc9f4a7bc7d77d12b488be2cf0bf79a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666989"
---
# <a name="mitigate-the-application-was-not-detected-error"></a><span data-ttu-id="51e33-102">Mitigar o erro "A aplicação não foi detetada"</span><span class="sxs-lookup"><span data-stu-id="51e33-102">Mitigate "The application was not detected" error</span></span>

<span data-ttu-id="51e33-103">O erro de instalação da aplicação, "A aplicação não foi detetada após a instalação ter sido concluída com êxito", reportado pelo Intune, pode ocorrer em todas as principais plataformas de SO (Windows, iOS e Android).</span><span class="sxs-lookup"><span data-stu-id="51e33-103">The app installation error, “The application was not detected after installation completed successfully,” reported by Intune, may occur on all major OS platforms (Windows, iOS and Android).</span></span>

<span data-ttu-id="51e33-104">Os cenários mais comuns que geram este erro incluem:</span><span class="sxs-lookup"><span data-stu-id="51e33-104">The most common scenarios that generate this error include:</span></span>

- <span data-ttu-id="51e33-105">A aplicação foi atualizada fora de Intune (a partir de uma loja de aplicações de terceiros) após a implementação inicial.</span><span class="sxs-lookup"><span data-stu-id="51e33-105">The app has been updated outside of Intune (from a third-party app store) after the initial deployment.</span></span> <span data-ttu-id="51e33-106">Por exemplo, algumas aplicações como o Google Chrome podem realizar atualizações automáticas.</span><span class="sxs-lookup"><span data-stu-id="51e33-106">For example some applications such as Google Chrome may perform auto updates.</span></span>
- <span data-ttu-id="51e33-107">Um utilizador desinstalou a aplicação após a instalação inicial.</span><span class="sxs-lookup"><span data-stu-id="51e33-107">A user has uninstalled the app after the initial install.</span></span>

<span data-ttu-id="51e33-108">Para mitigar este problema, reveja primeiro os dispositivos afetados para determinar o cenário em que o erro ocorre.</span><span class="sxs-lookup"><span data-stu-id="51e33-108">To mitigate this issue, first perform a review of the affected devices to determine the scenario in which the error occurs.</span></span>

- <span data-ttu-id="51e33-109">Se a aplicação tiver sido atualizada fora do Intune, a implementação da aplicação pode ser definida para ignorar a versão da aplicação.</span><span class="sxs-lookup"><span data-stu-id="51e33-109">If the app has been updated outside of Intune, the app deployment can be set to ignore the application version.</span></span> <span data-ttu-id="51e33-110">Para tal, em **Configuração da Aplicação > Informações da Aplicação**, defina **Ignorar a versão da aplicação** como **Sim**.</span><span class="sxs-lookup"><span data-stu-id="51e33-110">To do so, under **App Configuration > App Information**, set **Ignore App** version to **Yes**.</span></span>
- <span data-ttu-id="51e33-111">Ao focar-se no cliente, poderá ser apropriado implementar a aplicação como "necessária", e garantir que a versão mais recente é implementada.</span><span class="sxs-lookup"><span data-stu-id="51e33-111">When targeting the client, it may be appropriate to deploy the application as “required,” and to ensure that the latest version is deployed.</span></span>
- <span data-ttu-id="51e33-112">Em alternativa, na plataforma iOS, é possível utilizar a funcionalidade de **atualização automática** associada ao Programa de Compra em Volume da Apple, que pode ser configurada para atualizar automaticamente para novas versões de aplicações à medida que forem disponibilizadas.</span><span class="sxs-lookup"><span data-stu-id="51e33-112">Alternatively, on the iOS platform, it is possible to use the **autoupdate** functionality associated with the Apple Volume Purchase Program, which can be configured to automatically update to new application versions as they become available.</span></span>

<span data-ttu-id="51e33-113">Para obter mais informações sobre resolução de problemas de instalação de aplicações, consulte [Resolver problemas de instalação de aplicações](https://docs.microsoft.com/intune/troubleshoot-app-install).</span><span class="sxs-lookup"><span data-stu-id="51e33-113">For more information about troubleshooting app installation issues, please see [Troubleshoot app installation issues](https://docs.microsoft.com/intune/troubleshoot-app-install).</span></span>
