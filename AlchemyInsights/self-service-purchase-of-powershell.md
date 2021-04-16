---
title: Compra self-service da PowerShell
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
- "9001212"
- "3516"
ms.openlocfilehash: 48b5b0a1be1bc03d45a531a1093f18a3f750c37d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51797732"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="ca2de-102">Compra self-service da PowerShell</span><span class="sxs-lookup"><span data-stu-id="ca2de-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="ca2de-103">Para utilizar o módulo MSCommerce PowerShell, é necessário instalá-lo num dispositivo Windows 10 com TLS 1.2 (permissões de administrador local necessárias).</span><span class="sxs-lookup"><span data-stu-id="ca2de-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="ca2de-104">Importar e ligar ao módulo MSCommerce.</span><span class="sxs-lookup"><span data-stu-id="ca2de-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="ca2de-105">Quando solicitado para iniciar sessão, terá de usar credenciais de função Global ou Billing Admin.</span><span class="sxs-lookup"><span data-stu-id="ca2de-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="ca2de-106">Se não tiver TLS 1.2, poderá receber o seguinte erro ao tentar obter ou atualizar a política:</span><span class="sxs-lookup"><span data-stu-id="ca2de-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="ca2de-107">*ErrorMessage -A ligação subjacente foi encerrada: Ocorreu um erro inesperado num envio*.</span><span class="sxs-lookup"><span data-stu-id="ca2de-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>



