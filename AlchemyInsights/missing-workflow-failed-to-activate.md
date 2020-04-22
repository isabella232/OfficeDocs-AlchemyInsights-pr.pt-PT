---
title: Fluxo de trabalho desaparecido falhou em ativar
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 2598111005c219c398b63ca374e8e99348efc02c
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43762112"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="0e228-102">Fluxo de trabalho desaparecido falhou em ativar</span><span class="sxs-lookup"><span data-stu-id="0e228-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="0e228-103">Numa coleção de site do Microsoft SharePoint, não é possível adicionar um fluxo de trabalho globalmente reutilizável (como "Approval - SharePoint 2010") a uma lista ou biblioteca.</span><span class="sxs-lookup"><span data-stu-id="0e228-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="0e228-104">Para resolver esta questão, siga estes passos:</span><span class="sxs-lookup"><span data-stu-id="0e228-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="0e228-105">Abra o site raiz da coleção do site no SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="0e228-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="0e228-106">Sob **os Objetos do Site,** selecione **Fluxos de Trabalho**.</span><span class="sxs-lookup"><span data-stu-id="0e228-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="0e228-107">Na **nova** secção da fita **Workflows,** selecione Fluxos de **Trabalho Reutilizáveis**.</span><span class="sxs-lookup"><span data-stu-id="0e228-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="0e228-108">No formulário **Create Reutilable Workflow,** introduza o nome \*\* *Repair2010* \*\*.</span><span class="sxs-lookup"><span data-stu-id="0e228-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="0e228-109">Para **o Tipo de Plataforma,** clique no **SharePoint 2010 Workflow**, e depois clique em **OK**.</span><span class="sxs-lookup"><span data-stu-id="0e228-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="0e228-110">Na secção **Guardar** da fita **Workflow,** selecione **Publicar**.</span><span class="sxs-lookup"><span data-stu-id="0e228-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="0e228-111">Na secção **Gerir** a fita **Workflow,** selecione **Publicar Globalmente**.</span><span class="sxs-lookup"><span data-stu-id="0e228-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="0e228-112">Na caixa de diálogo de confirmação que aparece, selecione **OK**.</span><span class="sxs-lookup"><span data-stu-id="0e228-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="0e228-113">Num navegador web, localize o site raiz da coleção do site e, em seguida, aceda às **Funcionalidades**de Recolha do **Site** \> .</span><span class="sxs-lookup"><span data-stu-id="0e228-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="0e228-114">Em seguida, alternar a função **Workflows:**</span><span class="sxs-lookup"><span data-stu-id="0e228-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="0e228-115">· Se a funcionalidade for *Ativada,* clique em **Desativar** e, em seguida, clique em **Ativar**.</span><span class="sxs-lookup"><span data-stu-id="0e228-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="0e228-116">· Se a funcionalidade for *desativada,* clique **em Ativar**.</span><span class="sxs-lookup"><span data-stu-id="0e228-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="0e228-117">Para mais informações, consulte o [seguinte artigo](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="0e228-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

