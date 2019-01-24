---
title: Falta o fluxo de trabalho não conseguiu activar
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 33b92c2cae1f641b0cd88c82fd4ae5e8632d76c2
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/24/2019
ms.locfileid: "29483611"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="51a74-102">Falta o fluxo de trabalho não conseguiu activar</span><span class="sxs-lookup"><span data-stu-id="51a74-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="51a74-103">Uma colecção de sites do Microsoft SharePoint, não é possível adicionar um fluxo de trabalho reutilizável globalmente (por exemplo, "aprovação - SharePoint 2010") para uma lista ou biblioteca.</span><span class="sxs-lookup"><span data-stu-id="51a74-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="51a74-104">Para resolver este problema, siga estes passos:</span><span class="sxs-lookup"><span data-stu-id="51a74-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="51a74-105">Abra o Web site de raiz da colecção de sites no SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="51a74-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="51a74-106">Em **Objectos de Site**, seleccione os **fluxos de trabalho**.</span><span class="sxs-lookup"><span data-stu-id="51a74-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="51a74-107">Na secção **Novo** friso **fluxos de trabalho** , seleccione o **Fluxo de trabalho reutilizável**.</span><span class="sxs-lookup"><span data-stu-id="51a74-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="51a74-p101">No formulário **Criar fluxo de trabalho reutilizável** , introduza o nome \* \* *Repair2010* \* \*. Para **Tipo de plataforma**, faça clique sobre **o fluxo de trabalho do SharePoint 2010**e, em seguida, clique em **OK**.</span><span class="sxs-lookup"><span data-stu-id="51a74-p101">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*. For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="51a74-110">Na secção **Guardar** do Friso de **fluxo de trabalho** , seleccione **Publicar**.</span><span class="sxs-lookup"><span data-stu-id="51a74-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="51a74-p102">Na secção **Gerir** o Friso de **fluxo de trabalho** , seleccione **Publicar globalmente**. Na caixa de diálogo de confirmação que aparece, seleccione **' OK '**.</span><span class="sxs-lookup"><span data-stu-id="51a74-p102">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**. In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="51a74-p103">Num web browser, localize o Web site de raiz da colecção de sites e, em seguida, aceder a **Definições do Site** \> **Funcionalidades de colecção de sites**. Em seguida, activar/desactivar a funcionalidade de **fluxos de trabalho** :</span><span class="sxs-lookup"><span data-stu-id="51a74-p103">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**. Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="51a74-115">· Se a funcionalidade estiver *activada* , clique em **desativar** e, em seguida, clique em **Activar**.</span><span class="sxs-lookup"><span data-stu-id="51a74-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="51a74-116">· Se a funcionalidade de *Deactivated* , clique em **Activar**.</span><span class="sxs-lookup"><span data-stu-id="51a74-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="51a74-117">Para obter mais informações, consulte o seguinte [artigo](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="51a74-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

