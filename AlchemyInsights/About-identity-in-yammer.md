---
title: Sobre a identidade em Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: f417117acac4c3040932fc0a35e5d0b1c3709cd5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664181"
---
# <a name="about-identity-in-yammer"></a><span data-ttu-id="91d42-102">Sobre a identidade em Yammer</span><span class="sxs-lookup"><span data-stu-id="91d42-102">About identity in Yammer</span></span>

<span data-ttu-id="91d42-103">Recomenda-se que todas as redes tomem as seguintes medidas para evitar questões relacionadas com a identidade:</span><span class="sxs-lookup"><span data-stu-id="91d42-103">It is recommended that all networks take the following steps to avoid identity-related issues:</span></span>

1. <span data-ttu-id="91d42-104">Impor a identidade do Office 365 depois de ter disponibilizado as contas da Microsoft 365 para os utilizadores em Azure AD para garantir que todos os utilizadores acedam utilizando a sua conta primária da Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="91d42-104">Enforce Office 365 identity after provisioning Microsoft 365 accounts for users in Azure AD to ensure that all users sign in by using their primary Microsoft 365 account.</span></span> <span data-ttu-id="91d42-105">Para mais informações, consulte [a identidade do Enforce Office 365 para utilizadores da Yammer.](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity)</span><span class="sxs-lookup"><span data-stu-id="91d42-105">For more info, see [Enforce Office 365 identity for Yammer users](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span></span>
2. <span data-ttu-id="91d42-106">Consolidar várias redes Yammer.</span><span class="sxs-lookup"><span data-stu-id="91d42-106">Consolidate multiple Yammer networks.</span></span> <span data-ttu-id="91d42-107">As configurações legacy Yammer permitem que várias redes Yammer sejam ligadas a um inquilino.</span><span class="sxs-lookup"><span data-stu-id="91d42-107">Legacy Yammer configurations permit multiple Yammer networks to be connected to one tenant.</span></span> <span data-ttu-id="91d42-108">Para obter mais informações, consulte [a migração da Rede - Consolidar várias redes Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span><span class="sxs-lookup"><span data-stu-id="91d42-108">For more info, see [Network migration - Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>
3. <span data-ttu-id="91d42-109">Opcionalmente, imponha o licenciamento para a Yammer bloquear os utilizadores da Yammer se não tiverem licença.</span><span class="sxs-lookup"><span data-stu-id="91d42-109">Optionally, enforce licensing for Yammer to block users from Yammer if they don't have a license.</span></span> <span data-ttu-id="91d42-110">Para mais informações, consulte [as licenças de utilizador da Manage Yammer no Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="91d42-110">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span></span>
4. <span data-ttu-id="91d42-111">Por fim, audite a lista de utilizadores para redes Yammer mais antigas e suspenda os utilizadores antigos.</span><span class="sxs-lookup"><span data-stu-id="91d42-111">Finally, audit the user list for older Yammer networks and suspend legacy users.</span></span> <span data-ttu-id="91d42-112">Recomenda-se que suspenda (desativar) os utilizadores em vez de os eliminar, porque a eliminação é irreversível.</span><span class="sxs-lookup"><span data-stu-id="91d42-112">It is recommended that you suspend (deactivate) users instead of deleting them, because deletion is irreversible.</span></span> <span data-ttu-id="91d42-113">Para obter mais informações, consulte [os utilizadores da Audit Yammer em redes ligadas ao Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) e [remover os utilizadores.](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users)</span><span class="sxs-lookup"><span data-stu-id="91d42-113">For more info, see [Audit Yammer users in networks connected to Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) and [Remove users](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span></span>

<span data-ttu-id="91d42-114">Ao configurar o Yammer usando estes passos, também estará pronto para configurar a sua rede Yammer para Modo Nativo para a Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="91d42-114">By configuring Yammer using these steps, you'll also be ready to configure your Yammer network for Native Mode for Microsoft 365.</span></span> <span data-ttu-id="91d42-115">Para obter mais informações, consulte [configurar a sua rede Yammer para Modo Nativo para a Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span><span class="sxs-lookup"><span data-stu-id="91d42-115">For more info, see [Configure your Yammer network for Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span></span>