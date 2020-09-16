---
title: Compra self-service da PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3516"
ms.openlocfilehash: e6cc504ebef19cbe78f576d9b207fe2d951d0ef5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47739981"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="517fa-102">Compra self-service da PowerShell</span><span class="sxs-lookup"><span data-stu-id="517fa-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="517fa-103">Para utilizar o módulo MSCommerce PowerShell, é necessário instalá-lo num dispositivo Windows 10 com TLS 1.2 (permissões de administrador local necessárias).</span><span class="sxs-lookup"><span data-stu-id="517fa-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="517fa-104">Importar e ligar ao módulo MSCommerce.</span><span class="sxs-lookup"><span data-stu-id="517fa-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="517fa-105">Quando solicitado para iniciar sessão, terá de usar credenciais de função Global ou Billing Admin.</span><span class="sxs-lookup"><span data-stu-id="517fa-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="517fa-106">Se não tiver TLS 1.2, poderá receber o seguinte erro ao tentar obter ou atualizar a política:</span><span class="sxs-lookup"><span data-stu-id="517fa-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="517fa-107">*ErrorMessage -A ligação subjacente foi encerrada: Ocorreu um erro inesperado num envio*.</span><span class="sxs-lookup"><span data-stu-id="517fa-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>



