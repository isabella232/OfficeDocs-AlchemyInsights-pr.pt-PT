---
title: Falha no fluxo de trabalho ausente para ativar
ms.author: pebaum
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: f03d7e1441465050c4b0608f4100f217b183d2e2
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/18/2019
ms.locfileid: "36753807"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="b9de3-102">Falha no fluxo de trabalho ausente para ativar</span><span class="sxs-lookup"><span data-stu-id="b9de3-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="b9de3-103">Em um conjunto de sites do Microsoft SharePoint, você não pode adicionar um fluxo de trabalho globalmente reutilizável (como "aprovação-SharePoint 2010") a uma lista ou biblioteca.</span><span class="sxs-lookup"><span data-stu-id="b9de3-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="b9de3-104">Para resolver este problema, siga estes passos:</span><span class="sxs-lookup"><span data-stu-id="b9de3-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="b9de3-105">Abra o site raiz do conjunto de sites no SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="b9de3-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="b9de3-106">Em **objetos do site**, selecione **fluxos de trabalho**.</span><span class="sxs-lookup"><span data-stu-id="b9de3-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="b9de3-107">Na **nova** seção da faixa de opções **fluxos de trabalho** , selecione fluxo de **trabalho reutilizável**.</span><span class="sxs-lookup"><span data-stu-id="b9de3-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="b9de3-108">No formulário **criar fluxo de trabalho reutilizável** , digite o nome \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="b9de3-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="b9de3-109">Para **tipo de plataforma**, clique em **SharePoint 2010 Workflow**e, em seguida, clique em **OK**.</span><span class="sxs-lookup"><span data-stu-id="b9de3-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="b9de3-110">Na seção **salvar** da faixa de opções de **fluxo de trabalho** , selecione **publicar**.</span><span class="sxs-lookup"><span data-stu-id="b9de3-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="b9de3-111">Na seção **gerenciar** da faixa de opções **fluxo de trabalho** , selecione **publicar globalmente**.</span><span class="sxs-lookup"><span data-stu-id="b9de3-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="b9de3-112">Na caixa de diálogo de confirmação que aparece, selecione **OK**.</span><span class="sxs-lookup"><span data-stu-id="b9de3-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="b9de3-113">Em um navegador da Web, localize o site raiz do conjunto de sites e, em seguida, acesse **recursos de conjunto**de sites de **configurações** \> do site.</span><span class="sxs-lookup"><span data-stu-id="b9de3-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="b9de3-114">Em seguida, alterne o recurso de **fluxos de trabalho** :</span><span class="sxs-lookup"><span data-stu-id="b9de3-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="b9de3-115">· Se o recurso estiver *ativado* , clique em **desativar** e, em seguida, clique em **Ativar**.</span><span class="sxs-lookup"><span data-stu-id="b9de3-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="b9de3-116">· Se o recurso estiver *desativado* , clique em **Ativar**.</span><span class="sxs-lookup"><span data-stu-id="b9de3-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="b9de3-117">Para obter mais informações, consulte o seguinte [artigo](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="b9de3-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

