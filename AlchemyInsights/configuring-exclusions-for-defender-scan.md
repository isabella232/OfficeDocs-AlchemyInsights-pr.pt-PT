---
title: Configurar exclusões para o Microsoft Defender ATP scan
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6027"
- "9001464"
ms.openlocfilehash: 912e77b9b1a149fef373f2d0814fb2f0671a48c6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "50713902"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="961dd-102">Configurar exclusões para o Microsoft Defender ATP scan</span><span class="sxs-lookup"><span data-stu-id="961dd-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="961dd-103">Em geral, pode excluir determinadas extensões de ficheiros e localizações de pastas das verificações ATP do Microsoft Defender.</span><span class="sxs-lookup"><span data-stu-id="961dd-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="961dd-104">Também pode configurar exclusões para ficheiros abertos por determinados processos.</span><span class="sxs-lookup"><span data-stu-id="961dd-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="961dd-105">Para obter mais informações, consulte, [configuure e valide exclusões com base na extensão de ficheiros e localização de pastas](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) e [exclusões de configuração para ficheiros abertos por processos](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span><span class="sxs-lookup"><span data-stu-id="961dd-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="961dd-106">Para configurar as exclusões para  **o Windows Server 2016 e 2019**, consulte [exclusões antivírus do Microsoft Defender no Windows Server](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="961dd-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="961dd-107">**Mac**</span><span class="sxs-lookup"><span data-stu-id="961dd-107">**Mac**</span></span>

<span data-ttu-id="961dd-108">Para obter detalhes sobre tipos de exclusão suportados e configurar uma lista de exclusões para Mac, consulte tipos de [exclusão suportados](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) e [como configurar a lista de exclusões](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span><span class="sxs-lookup"><span data-stu-id="961dd-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="961dd-109">**Nota** Também pode validar listas de exclusões utilizando o ficheiro de teste EICAR.</span><span class="sxs-lookup"><span data-stu-id="961dd-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="961dd-110">Para obter mais informações, consulte [validar as listas de exclusões com o ficheiro de teste EICAR](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span><span class="sxs-lookup"><span data-stu-id="961dd-110">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="961dd-111">**Linux**</span><span class="sxs-lookup"><span data-stu-id="961dd-111">**Linux**</span></span>

<span data-ttu-id="961dd-112">Para obter detalhes sobre tipos de exclusão suportados e configurar uma lista de exclusões para o Linux, consulte tipos de [exclusão suportados](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) e [configurar e validar exclusões para o Microsoft Defender ATP para o Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span><span class="sxs-lookup"><span data-stu-id="961dd-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="961dd-113">**Nota** Também pode validar listas de exclusões utilizando o ficheiro de teste EICAR.</span><span class="sxs-lookup"><span data-stu-id="961dd-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="961dd-114">Para obter mais informações, consulte [validar as listas de exclusões com o ficheiro de teste EICAR](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span><span class="sxs-lookup"><span data-stu-id="961dd-114">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 