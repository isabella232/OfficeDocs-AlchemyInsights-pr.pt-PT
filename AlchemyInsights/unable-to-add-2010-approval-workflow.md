---
title: Não é possível adicionar o fluxo de trabalho de aprovação de 2010
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: a83a9621ca0f7764d3f2c0a698dbffd80d55e80c
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/15/2019
ms.locfileid: "28306454"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="4ec8c-102">Não é possível adicionar o fluxo de trabalho de aprovação de 2010</span><span class="sxs-lookup"><span data-stu-id="4ec8c-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="4ec8c-103">Uma colecção de sites do Microsoft SharePoint, não é possível adicionar um fluxo de trabalho reutilizável globalmente (por exemplo, "aprovação - SharePoint 2010") para uma lista ou biblioteca.</span><span class="sxs-lookup"><span data-stu-id="4ec8c-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="4ec8c-104">Para resolver este problema, siga estes passos:</span><span class="sxs-lookup"><span data-stu-id="4ec8c-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="4ec8c-105">Abra o Web site de raiz da colecção de sites no SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="4ec8c-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="4ec8c-106">Em **Objectos de Site**, seleccione os **fluxos de trabalho**.</span><span class="sxs-lookup"><span data-stu-id="4ec8c-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="4ec8c-107">Na secção **Novo** friso **fluxos de trabalho** , seleccione o **Fluxo de trabalho reutilizável**.</span><span class="sxs-lookup"><span data-stu-id="4ec8c-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="4ec8c-p101">No formulário **Criar fluxo de trabalho reutilizável** , introduza o nome \* \* *Repair2010* \* \*. Para **Tipo de plataforma**, faça clique sobre **o fluxo de trabalho do SharePoint 2010**e, em seguida, clique em **OK**.</span><span class="sxs-lookup"><span data-stu-id="4ec8c-p101">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*. For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="4ec8c-110">Na secção **Guardar** do Friso de **fluxo de trabalho** , seleccione **Publicar**.</span><span class="sxs-lookup"><span data-stu-id="4ec8c-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="4ec8c-p102">Na secção **Gerir** o Friso de **fluxo de trabalho** , seleccione **Publicar globalmente**. Na caixa de diálogo de confirmação que aparece, seleccione **' OK '**.</span><span class="sxs-lookup"><span data-stu-id="4ec8c-p102">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**. In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="4ec8c-p103">Num web browser, localize o Web site de raiz da colecção de sites e, em seguida, aceder a **Definições do Site** \> **Funcionalidades de colecção de sites**. Activar/desactivar a funcionalidade de **fluxos de trabalho** :</span><span class="sxs-lookup"><span data-stu-id="4ec8c-p103">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**. Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="4ec8c-115">· Se a funcionalidade estiver *activada* , clique em **desativar** e, em seguida, clique em **Activar**.</span><span class="sxs-lookup"><span data-stu-id="4ec8c-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="4ec8c-116">· Se a funcionalidade de *Deactivated* , clique em **Activar**.</span><span class="sxs-lookup"><span data-stu-id="4ec8c-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="4ec8c-117">Para obter mais informações, consulte o seguinte [artigo](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="4ec8c-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

