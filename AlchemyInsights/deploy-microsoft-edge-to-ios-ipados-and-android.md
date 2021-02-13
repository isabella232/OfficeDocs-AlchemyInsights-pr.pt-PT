---
title: Implementar o Microsoft Edge para iOS, iPadOS e Android
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
- "8241"
- "9004604"
ms.openlocfilehash: 524e87ab57e29823361053093708c83831f19687
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/10/2021
ms.locfileid: "50194591"
---
# <a name="deploy-microsoft-edge-to-ios-ipados-and-android"></a><span data-ttu-id="5fe37-102">Implementar o Microsoft Edge para iOS, iPadOS e Android</span><span class="sxs-lookup"><span data-stu-id="5fe37-102">Deploy Microsoft Edge to iOS, iPadOS, and Android</span></span>

<span data-ttu-id="5fe37-103">O cenário guiado resumido abaixo irá ajudá-lo a atribuir o Microsoft Edge aos utilizadores de dispositivos iOS, iPadOS e Android.</span><span class="sxs-lookup"><span data-stu-id="5fe37-103">The guided scenario summarized below will help you assign Microsoft Edge to users of iOS, iPadOS, and Android devices.</span></span>

> [!NOTE]
> <span data-ttu-id="5fe37-104">Se bloqueou os utilizadores da inscrição de dispositivos móveis, este cenário guiado não funcionará e os utilizadores terão de instalar o Microsoft Edge por si próprios.</span><span class="sxs-lookup"><span data-stu-id="5fe37-104">If you blocked users from enrolling mobile devices, this guided scenario won't work and the users will need to install Microsoft Edge on their own.</span></span>

<span data-ttu-id="5fe37-105">O cenário orientado envolve os seguintes passos:</span><span class="sxs-lookup"><span data-stu-id="5fe37-105">The guided scenario involves the following steps:</span></span>

1. [<span data-ttu-id="5fe37-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5fe37-106">Prerequisites</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#prerequisites)
2. [<span data-ttu-id="5fe37-107">Introdução</span><span class="sxs-lookup"><span data-stu-id="5fe37-107">Introduction</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-1---introduction)
3. [<span data-ttu-id="5fe37-108">Básico</span><span class="sxs-lookup"><span data-stu-id="5fe37-108">Basics</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-2---basics)
4. [<span data-ttu-id="5fe37-109">Configuração</span><span class="sxs-lookup"><span data-stu-id="5fe37-109">Configuration</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-3---configuration)
5. [<span data-ttu-id="5fe37-110">Atribuições</span><span class="sxs-lookup"><span data-stu-id="5fe37-110">Assignments</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-4---assignments)
6. [<span data-ttu-id="5fe37-111">Revisão e criação</span><span class="sxs-lookup"><span data-stu-id="5fe37-111">Review and creation</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-5---review--create)

<span data-ttu-id="5fe37-112">Depois de completar os passos no cenário guiado, as políticas do Microsoft Intune permitirão as seguintes funcionalidades do Microsoft Edge para negócios:</span><span class="sxs-lookup"><span data-stu-id="5fe37-112">After you complete the steps in the guided scenario, Microsoft Intune policies will enable the following features of Microsoft Edge for business:</span></span>

- <span data-ttu-id="5fe37-113">Dupla identidade</span><span class="sxs-lookup"><span data-stu-id="5fe37-113">Dual identity</span></span>
- <span data-ttu-id="5fe37-114">Integração com a política de proteção de aplicações microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="5fe37-114">Integration with Microsoft Intune app protection policy</span></span>
- <span data-ttu-id="5fe37-115">Integração com a Azure Ative Directory Application Proxy</span><span class="sxs-lookup"><span data-stu-id="5fe37-115">Integration with Azure Active Directory Application Proxy</span></span>
- <span data-ttu-id="5fe37-116">Favoritos geridos e atalhos de página inicial</span><span class="sxs-lookup"><span data-stu-id="5fe37-116">Managed favorites and home page shortcuts</span></span>
