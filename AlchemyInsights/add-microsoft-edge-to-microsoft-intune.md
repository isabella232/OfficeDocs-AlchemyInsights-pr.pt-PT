---
title: Adicione o Microsoft Edge ao Microsoft Intune
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8240"
- "9004604"
ms.openlocfilehash: d56c65910d1c2170d3e0ce9676e913663701db96
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/10/2021
ms.locfileid: "50194572"
---
# <a name="add-microsoft-edge-to-microsoft-intune"></a><span data-ttu-id="4f851-102">Adicione o Microsoft Edge ao Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="4f851-102">Add Microsoft Edge to Microsoft Intune</span></span>

<span data-ttu-id="4f851-103">Para poder implementar, configurar, monitorizar e proteger o Microsoft Edge para o Windows 10, tem primeiro de o adicionar ao Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="4f851-103">To be able to deploy, configure, monitor, and protect Microsoft Edge for Windows 10, you must first add it to Microsoft Intune.</span></span>

> [!IMPORTANT]
- <span data-ttu-id="4f851-104">Intune suporta as versões Microsoft Edge 77 e posteriores.</span><span class="sxs-lookup"><span data-stu-id="4f851-104">Intune supports Microsoft Edge 77 and later versions.</span></span>
- <span data-ttu-id="4f851-105">A Intune detetará quaisquer instalações pré-existentes do Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="4f851-105">Intune will detect any pre-existing installations of Microsoft Edge.</span></span>
- <span data-ttu-id="4f851-106">Se o Microsoft Edge for instalado no contexto do utilizador, uma instalação do sistema substituirá a instalação no contexto do utilizador.</span><span class="sxs-lookup"><span data-stu-id="4f851-106">If Microsoft Edge is installed in user context, a system installation will overwrite the installation in user context.</span></span>
- <span data-ttu-id="4f851-107">Se o Microsoft Edge for instalado em contexto de sistema, o sucesso da instalação será reportado.</span><span class="sxs-lookup"><span data-stu-id="4f851-107">If Microsoft Edge is installed in system context, the installation success will be reported.</span></span>
- <span data-ttu-id="4f851-108">As versões pré-instaladas do Microsoft Edge 77 e posteriores, para todos os canais em contexto de utilizador, serão substituídas com o Microsoft Edge instalado em contexto de sistema.</span><span class="sxs-lookup"><span data-stu-id="4f851-108">Pre-installed Microsoft Edge 77 and later versions, for all channels in user context, will be overwritten with Microsoft Edge installed in system context.</span></span>

<span data-ttu-id="4f851-109">**Pré-requisito**</span><span class="sxs-lookup"><span data-stu-id="4f851-109">**Prerequisite**</span></span>

<span data-ttu-id="4f851-110">Versões 1709 ou posterior do Windows 10</span><span class="sxs-lookup"><span data-stu-id="4f851-110">Windows 10 version 1709 or later versions</span></span>

<span data-ttu-id="4f851-111">**Passos para adicionar Edge ao Intune**</span><span class="sxs-lookup"><span data-stu-id="4f851-111">**Steps to add Edge to Intune**</span></span>

1. <span data-ttu-id="4f851-112">[Configure a aplicação em Intune](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="4f851-112">[Configure the app in Intune](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
2. <span data-ttu-id="4f851-113">[Configure a informação da aplicação.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="4f851-113">[Configure the app information](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
3. <span data-ttu-id="4f851-114">[Configure as definições da aplicação](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="4f851-114">[Configure the app settings](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
4. <span data-ttu-id="4f851-115">[Selecione as etiquetas de âmbito (opcional)](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="4f851-115">[Select the scope tags (optional)](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
5. <span data-ttu-id="4f851-116">[Adicione a aplicação.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="4f851-116">[Add the app](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>

<span data-ttu-id="4f851-117">Para obter mais ajuda, consulte [a resolução de problemas.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="4f851-117">For more help, see [Troubleshooting](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>




