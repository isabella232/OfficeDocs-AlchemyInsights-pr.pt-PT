---
title: Código de erro 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Se estiver a receber um erro ao activar o Office 2013 em implementações de serviços de ambiente de trabalho remoto (RDS), considere a activação ADAL editando o registo.
ms.openlocfilehash: e2249d8ebbd2313c64dda5656a3243fa76d97a9a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/28/2019
ms.locfileid: "35388256"
---
<span data-ttu-id="55c84-103">Se estiver a receber um erro ao activar o Office 2013 em implementações de serviços de ambiente de trabalho remoto (RDS), considere a activação ADAL editando o registo.</span><span class="sxs-lookup"><span data-stu-id="55c84-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="55c84-104">**Chave de registo**</span><span class="sxs-lookup"><span data-stu-id="55c84-104">**Registry key**</span></span>|<span data-ttu-id="55c84-105">**Tipo**</span><span class="sxs-lookup"><span data-stu-id="55c84-105">**Type**</span></span>|<span data-ttu-id="55c84-106">**Valor**</span><span class="sxs-lookup"><span data-stu-id="55c84-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="55c84-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="55c84-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="55c84-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="55c84-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="55c84-109">1</span><span class="sxs-lookup"><span data-stu-id="55c84-109">1</span></span>  <br/> |

<span data-ttu-id="55c84-110">Para mais informações, consulte [Activar autenticação moderna para 2013 do Office em dispositivos do Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="55c84-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="55c84-111">ADAL está activado por predefinição no Office 365 ProPlus e de 2016 Office.</span><span class="sxs-lookup"><span data-stu-id="55c84-111">ADAL is enabled by default in Office 365 ProPlus and Office 2016.</span></span> <span data-ttu-id="55c84-112">> serviços de ambiente de trabalho remoto (RDS) era anteriormente chamado dos serviços de Terminal.</span><span class="sxs-lookup"><span data-stu-id="55c84-112">>  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  