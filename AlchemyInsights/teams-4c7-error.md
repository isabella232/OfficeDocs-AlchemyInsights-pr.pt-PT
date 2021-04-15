---
title: Erro das equipas 4c7
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 51f2aa936e803b63bcbdf73b89959cd3a1757751
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786680"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="69a32-102">Erro 4c7 nas Equipas da Microsoft</span><span class="sxs-lookup"><span data-stu-id="69a32-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="69a32-103">Este erro ocorre porque as equipas da Microsoft requerem autenticação de formulários.</span><span class="sxs-lookup"><span data-stu-id="69a32-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="69a32-104">Quando implementa serviços da Federação de Diretórios Ativos (AD FS), a autenticação de formulários não está ativada para a intranet por predefinição.</span><span class="sxs-lookup"><span data-stu-id="69a32-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="69a32-105">Se a autenticação integrada do Windows falhar, é-lhe pedido que faça sedutação utilizando a Autenticação de Formulários.</span><span class="sxs-lookup"><span data-stu-id="69a32-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="69a32-106">Para resolver este problema, ative a autenticação de formulários utilizando o encaixe da Consola de Gestão da Microsoft (MMC) AD FS no computador que tem a cópia local do Ative Directory.</span><span class="sxs-lookup"><span data-stu-id="69a32-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="69a32-107">Para tal, siga estes passos:</span><span class="sxs-lookup"><span data-stu-id="69a32-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="69a32-108">No painel de navegação, procure políticas **de autenticação.**</span><span class="sxs-lookup"><span data-stu-id="69a32-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="69a32-109">Em **Ações** no painel de detalhes, **selecione Editar Autenticação Primária Global.**</span><span class="sxs-lookup"><span data-stu-id="69a32-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="69a32-110">No separador **Intranet,** selecione **Autenticação de Formulários.**</span><span class="sxs-lookup"><span data-stu-id="69a32-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="69a32-111">Selecione **OK** (ou **Aplique).**</span><span class="sxs-lookup"><span data-stu-id="69a32-111">Select **OK** (or **Apply**).</span></span>