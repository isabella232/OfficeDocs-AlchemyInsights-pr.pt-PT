---
title: Código de erro 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Se estiver a receber um erro ao activar o Office 2013 em implementações de serviços de ambiente de trabalho remoto (RDS), considere a activação ADAL editando o registo.
ms.openlocfilehash: 6d4076ecb5c6ee3c3cf4c4610ad4aa29ab477d8a
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32402750"
---
<span data-ttu-id="6809b-103">Se estiver a receber um erro ao activar o Office 2013 em implementações de serviços de ambiente de trabalho remoto (RDS), considere a activação ADAL editando o registo.</span><span class="sxs-lookup"><span data-stu-id="6809b-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span> 
  
|<span data-ttu-id="6809b-104">**Chave de registo**</span><span class="sxs-lookup"><span data-stu-id="6809b-104">**Registry key**</span></span>|<span data-ttu-id="6809b-105">**Tipo**</span><span class="sxs-lookup"><span data-stu-id="6809b-105">**Type**</span></span>|<span data-ttu-id="6809b-106">**Valor**</span><span class="sxs-lookup"><span data-stu-id="6809b-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="6809b-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="6809b-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="6809b-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="6809b-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="6809b-109">1</span><span class="sxs-lookup"><span data-stu-id="6809b-109">1</span></span>  <br/> |
   
<span data-ttu-id="6809b-110">Para mais informações, consulte [Activar autenticação moderna para 2013 do Office em dispositivos do Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="6809b-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="6809b-111">ADAL está activado por predefinição no Office 365 ProPlus e de 2016 Office.</span><span class="sxs-lookup"><span data-stu-id="6809b-111">ADAL is enabled by default in Office 365 ProPlus and Office 2016.</span></span> <span data-ttu-id="6809b-112">> serviços de ambiente de trabalho remoto (RDS) era anteriormente chamado dos serviços de Terminal.</span><span class="sxs-lookup"><span data-stu-id="6809b-112">>  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span> 
  

