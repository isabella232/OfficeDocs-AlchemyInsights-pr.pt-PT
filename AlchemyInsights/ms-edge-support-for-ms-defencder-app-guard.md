---
title: Suporte do Microsoft Edge para Microsoft Defender Application Guard
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004024"
- "7090"
ms.openlocfilehash: 65cbc867ea7d1c73ca2906f51f72aa3376f31b5d
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/04/2020
ms.locfileid: "49584014"
---
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a><span data-ttu-id="22a66-102">Suporte do Microsoft Edge para Microsoft Defender Application Guard</span><span class="sxs-lookup"><span data-stu-id="22a66-102">Microsoft Edge's support for Microsoft Defender Application Guard</span></span>

<span data-ttu-id="22a66-103">Projetado para o Windows 10 e Microsoft Edge, o Application Guard utiliza uma abordagem de isolamento de hardware que permite ao utilizador navegar num site não fideducionado a partir de dentro de um recipiente isolado, ativado por Hiper-V, separado do sistema operativo anfitrião.</span><span class="sxs-lookup"><span data-stu-id="22a66-103">Designed for Windows 10 and Microsoft Edge, Application Guard uses a hardware-isolation approach that lets a user navigate an untrusted site from inside an isolated, Hyper-V–enabled container, separated from the host operating system.</span></span>

<span data-ttu-id="22a66-104">Um administrador da empresa define uma lista de sites fidedignos, recursos em nuvem e redes internas.</span><span class="sxs-lookup"><span data-stu-id="22a66-104">An enterprise admin defines a list of trusted websites, cloud resources, and internal networks.</span></span> <span data-ttu-id="22a66-105">Quando um utilizador visita um site que não está na lista, o Microsoft Edge abrirá o site no contentor.</span><span class="sxs-lookup"><span data-stu-id="22a66-105">When a user visits a site that's not on the list, Microsoft Edge will open the site in the container.</span></span> <span data-ttu-id="22a66-106">Isto significa que se o site se revelar malicioso, o PC anfitrião permanecerá protegido e o intruso não chegará aos dados da empresa.</span><span class="sxs-lookup"><span data-stu-id="22a66-106">This means that if the site turns out to be malicious, the host PC will remain protected and the attacker won't get to the enterprise data.</span></span>

<span data-ttu-id="22a66-107">A instalação de extensões no contentor é suportada a partir da versão 81 do Microsoft Edge, e pode ser controlada através de uma política.</span><span class="sxs-lookup"><span data-stu-id="22a66-107">Installation of extensions in the container is supported as of Microsoft Edge version 81, and it can be controlled via a policy.</span></span> <span data-ttu-id="22a66-108">O endereço updateURL que é utilizado na política ExtensionInstallForcelist deve ser adicionado como um Recurso Neutro nas políticas de isolamento de rede utilizadas pela Guard de aplicação.</span><span class="sxs-lookup"><span data-stu-id="22a66-108">The updateURL address that gets used in the ExtensionInstallForcelist policy should be added as a Neutral Resource in the Network Isolation policies used by Application Guard.</span></span>

<span data-ttu-id="22a66-109">Para obter mais informações, consulte [o suporte do Microsoft Edge para o Microsoft Defender Application Guard](https://go.microsoft.com/fwlink/?linkid=2134229).</span><span class="sxs-lookup"><span data-stu-id="22a66-109">For more info, see [Microsoft Edge support for Microsoft Defender Application Guard](https://go.microsoft.com/fwlink/?linkid=2134229).</span></span>
