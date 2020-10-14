---
title: Implementação de aplicativo Intune Win32
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/06/2020
ms.locfileid: "48461876"
---
# <a name="intune-win32-app-deployment"></a><span data-ttu-id="93158-102">Implementação de aplicativo Intune Win32</span><span class="sxs-lookup"><span data-stu-id="93158-102">Intune Win32 app deployment</span></span>

<span data-ttu-id="93158-103">O Microsoft Intune permite aplicações Win32, incluindo, mas não se limitando a MSI e . O EXE vai ser implantado nos dispositivos do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="93158-103">Microsoft Intune allows Win32 applications, including but not limited to MSI and .EXE’s to be deployed to Windows 10 devices.</span></span> <span data-ttu-id="93158-104">O mecanismo de implantação utilizado requer a presença da Extensão de Gestão intune (IME) no dispositivo-alvo.</span><span class="sxs-lookup"><span data-stu-id="93158-104">The deployment mechanism used requires the Intune Management Extension (IME) to be present on the target device.</span></span> <span data-ttu-id="93158-105">O IME será instalado automaticamente como resultado de uma configuração de configuração ou implementação de aplicação win32 para um utilizador/dispositivo.</span><span class="sxs-lookup"><span data-stu-id="93158-105">The IME will be installed automatically as a result of targeting a powershell script or win32 application deployment to a user / device.</span></span>

<span data-ttu-id="93158-106">Há também um conjunto de pré-requisitos que devem ser cumpridos para implementar aplicações Win32 que incluem:</span><span class="sxs-lookup"><span data-stu-id="93158-106">There are also a set of pre-requisites which must be met in order to deploy Win32 apps which include:</span></span>

- <span data-ttu-id="93158-107">Plataformas suportadas: Versão 1607 ou posterior do Windows 10 (versões Enterprise, Pro e Education).</span><span class="sxs-lookup"><span data-stu-id="93158-107">Supported platforms: Windows 10 version 1607 or later (Enterprise, Pro, and Education versions).</span></span>
- <span data-ttu-id="93158-108">Arquitetura suportada: x86 e x64.</span><span class="sxs-lookup"><span data-stu-id="93158-108">Supported architecture: x86 and x64.</span></span>
- <span data-ttu-id="93158-109">Gestão de Dispositivos: AAD aderiu e matriculada automaticamente (incluindo domínio híbrido e política de grupo auto-inscrita).</span><span class="sxs-lookup"><span data-stu-id="93158-109">Device Management: AAD joined and auto-enrolled (including hybrid domain joined and group policy auto-enrolled).</span></span>
- <span data-ttu-id="93158-110">Formato pacote de aplicação: . **ficheiro intunewin**  preparado pela ferramenta de preparação de [conteúdo microsoft Win32](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).</span><span class="sxs-lookup"><span data-stu-id="93158-110">Application Package format: .**intunewin**  file prepared by the [Microsoft Win32 content Prep tool](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).</span></span>
- <span data-ttu-id="93158-111">Limitações:</span><span class="sxs-lookup"><span data-stu-id="93158-111">Limitations:</span></span>
    - <span data-ttu-id="93158-112">Tamanho máximo: 8GB.</span><span class="sxs-lookup"><span data-stu-id="93158-112">Maximum size: 8GB.</span></span>
    - <span data-ttu-id="93158-113">Arquitetura não suportada: ARMs.</span><span class="sxs-lookup"><span data-stu-id="93158-113">Unsupported architecture: ARMs.</span></span>

<span data-ttu-id="93158-114">Reveja o doc "[Add, assign, and monitor a Win32 app in Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" para obter informações relacionadas com esses passos.</span><span class="sxs-lookup"><span data-stu-id="93158-114">Review the doc "[Add, assign, and monitor a Win32 app in Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" for information related to those steps.</span></span>

<span data-ttu-id="93158-115">Os detalhes sobre a implementação de aplicações de resolução de problemas no Windows, incluindo aplicações Win32, podem ser revistos nos seguintes documentos</span><span class="sxs-lookup"><span data-stu-id="93158-115">Details on troubleshooting application deployment on Windows including Win32 apps can be reviewed in the following documents</span></span>

- [<span data-ttu-id="93158-116">Problemas de instalação de aplicativos de resolução de problemas</span><span class="sxs-lookup"><span data-stu-id="93158-116">Troubleshoot App Installation issues</span></span>](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [<span data-ttu-id="93158-117">Resolução de problemas Aplicativos Win32</span><span class="sxs-lookup"><span data-stu-id="93158-117">Troubleshoot Win32 Apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)