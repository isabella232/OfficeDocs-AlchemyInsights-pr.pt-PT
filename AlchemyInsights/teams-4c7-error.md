---
title: Equipes 4c7 erro
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 0945a341c6456ee4178c0485f3bfb9232fa78a11
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796296"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="5d125-102">Erro de 4c7 em equipes de Microsoft</span><span class="sxs-lookup"><span data-stu-id="5d125-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="5d125-103">Esse erro ocorre porque o Microsoft Teams requer autenticação de formulários.</span><span class="sxs-lookup"><span data-stu-id="5d125-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="5d125-104">Quando você implanta serviços da Federação de Direção Ativa (AD FS), a autenticação de formulários não é ativada para a intranet por padrão.</span><span class="sxs-lookup"><span data-stu-id="5d125-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="5d125-105">Se a autenticação integrada do Windows falhar, você será solicitado a entrar usando a autenticação de formulários.</span><span class="sxs-lookup"><span data-stu-id="5d125-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="5d125-106">Para resolver esse problema, habilite a autenticação de formulários usando o snap-in do AD FS Microsoft Management Console (MMC) no computador que tem a cópia local do Diretório Ativo.</span><span class="sxs-lookup"><span data-stu-id="5d125-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="5d125-107">To do this, follow these steps:</span><span class="sxs-lookup"><span data-stu-id="5d125-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="5d125-108">No painel de navegação, procure as Políticas de **Autenticação.**</span><span class="sxs-lookup"><span data-stu-id="5d125-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="5d125-109">**ações** no painel de detalhes, selecione **Eitie Autenticação Primária Global**.</span><span class="sxs-lookup"><span data-stu-id="5d125-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="5d125-110">Na guia **Intranet,** selecione **Autenticação de Formulários**.</span><span class="sxs-lookup"><span data-stu-id="5d125-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="5d125-111">Selecione **OK** (ou **Inscreva-se).**</span><span class="sxs-lookup"><span data-stu-id="5d125-111">Select **OK** (or **Apply**).</span></span>