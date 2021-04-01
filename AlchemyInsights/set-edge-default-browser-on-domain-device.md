---
title: Desafine o Microsoft Edge como o navegador predefinido num dispositivo ligado ao domínio
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: f51a455ea15b7bd92f548f2c1717be9888b43d07
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/30/2021
ms.locfileid: "51491882"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-domain-joined-device"></a><span data-ttu-id="e35f6-102">Desafine o Microsoft Edge como o navegador predefinido num dispositivo ligado ao domínio</span><span class="sxs-lookup"><span data-stu-id="e35f6-102">Set Microsoft Edge as the default browser on a domain-joined device</span></span>

<span data-ttu-id="e35f6-103">Desafine o Microsoft Edge como o navegador predefinido:</span><span class="sxs-lookup"><span data-stu-id="e35f6-103">Set Microsoft Edge as the default browser:</span></span> 

1. <span data-ttu-id="e35f6-104">[Crie um ficheiro de configuração de associações predefinido](https://go.microsoft.com/fwlink/?linkid=2132437) e armazene-o localmente ou numa partilha de rede.</span><span class="sxs-lookup"><span data-stu-id="e35f6-104">[Create a default associations configuration file](https://go.microsoft.com/fwlink/?linkid=2132437) and store it locally or on a network share.</span></span>

1. <span data-ttu-id="e35f6-105">Abra o editor de Política de Grupo e, em seguida, vá para **o Explorador**  >  **de**  >  **Ficheiros de Componentes do Windows de** configuração de  >  computador.</span><span class="sxs-lookup"><span data-stu-id="e35f6-105">Open the Group Policy editor, and then go to **Computer Configuration** > **Administrative Templates** > **Windows Components** > **File Explorer**.</span></span>

1. <span data-ttu-id="e35f6-106">Selecione **Definir um ficheiro de configuração de associações predefinidos**.</span><span class="sxs-lookup"><span data-stu-id="e35f6-106">Select **Set a default associations configuration file**.</span></span>

1. <span data-ttu-id="e35f6-107">Selecione **a definição de Política** e, em seguida, selecione **Ativado**.</span><span class="sxs-lookup"><span data-stu-id="e35f6-107">Select **Policy setting**, and then select **Enabled**.</span></span>

1. <span data-ttu-id="e35f6-108">Em **Opções**, insira a localização do ficheiro de configuração das suas associações predefinidos e, em seguida, selecione **OK**.</span><span class="sxs-lookup"><span data-stu-id="e35f6-108">Under **Options**, enter the location of your default associations configuration file, and then select **OK**.</span></span>
