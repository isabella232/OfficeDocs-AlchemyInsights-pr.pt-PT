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
ms.openlocfilehash: 4ef2943e5a529368fa2c614e4431cf180924fbb8
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36527042"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="c7ae5-103">Erro durante a activação do Office 2013 nos serviços de ambiente de trabalho remoto</span><span class="sxs-lookup"><span data-stu-id="c7ae5-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="c7ae5-104">Se estiver a receber um erro ao activar o Office 2013 em implementações de serviços de ambiente de trabalho remoto (RDS), considere a activação ADAL editando o registo.</span><span class="sxs-lookup"><span data-stu-id="c7ae5-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="c7ae5-105">**Chave de registo**</span><span class="sxs-lookup"><span data-stu-id="c7ae5-105">**Registry key**</span></span>|<span data-ttu-id="c7ae5-106">**Tipo**</span><span class="sxs-lookup"><span data-stu-id="c7ae5-106">**Type**</span></span>|<span data-ttu-id="c7ae5-107">**Valor**</span><span class="sxs-lookup"><span data-stu-id="c7ae5-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="c7ae5-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="c7ae5-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="c7ae5-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="c7ae5-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="c7ae5-110">1</span><span class="sxs-lookup"><span data-stu-id="c7ae5-110">1</span></span>  <br/> |

<span data-ttu-id="c7ae5-111">Para mais informações, consulte [Activar autenticação moderna para 2013 do Office em dispositivos do Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="c7ae5-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="c7ae5-112">ADAL está activado por predefinição no Office 365 ProPlus e de 2016 Office.</span><span class="sxs-lookup"><span data-stu-id="c7ae5-112">ADAL is enabled by default in Office 365 ProPlus and Office 2016.</span></span> <span data-ttu-id="c7ae5-113">Serviços de ambiente de trabalho remoto (RDS) era anteriormente chamado dos serviços de Terminal.</span><span class="sxs-lookup"><span data-stu-id="c7ae5-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  