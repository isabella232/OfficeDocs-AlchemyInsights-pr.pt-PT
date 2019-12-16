---
title: Incapaz de adicionar o fluxo de trabalho de aprovação de 2010
ms.author: pebaum
author: pebaum
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: 11ba9bf04f826b0d7465a9a81a36c327e79f4d13
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049564"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="8aaf2-102">Incapaz de adicionar o fluxo de trabalho de aprovação de 2010</span><span class="sxs-lookup"><span data-stu-id="8aaf2-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="8aaf2-103">Em uma coleção de sites do Microsoft SharePoint, você não pode adicionar um fluxo de trabalho globalmente reutilizável (como "Aprovação - SharePoint 2010") a uma lista ou biblioteca.</span><span class="sxs-lookup"><span data-stu-id="8aaf2-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="8aaf2-104">Para resolver este problema, siga estas etapas:</span><span class="sxs-lookup"><span data-stu-id="8aaf2-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="8aaf2-105">Abra o site raiz da coleção do site em SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="8aaf2-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="8aaf2-106">**objetos do site,** selecione fluxos de **trabalho.**</span><span class="sxs-lookup"><span data-stu-id="8aaf2-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="8aaf2-107">Na **nova** seção da fita **workflows,** selecione fluxo de **trabalho reutilizável.**</span><span class="sxs-lookup"><span data-stu-id="8aaf2-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="8aaf2-108">No formulário criar fluxo de **trabalho reutilizável,** digite o nome \*\* *Repair2010* \*\*.</span><span class="sxs-lookup"><span data-stu-id="8aaf2-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="8aaf2-109">Para **o tipo de plataforma,** clique no fluxo de trabalho **sharepoint 2010**e, em seguida, clique na **OK.**</span><span class="sxs-lookup"><span data-stu-id="8aaf2-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="8aaf2-110">Na seção **Save** da fita **workflow,** **selecione Publicar**.</span><span class="sxs-lookup"><span data-stu-id="8aaf2-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="8aaf2-111">Na seção **gerenciar** da fita **workflow,** selecione **Publicar Globalmente**.</span><span class="sxs-lookup"><span data-stu-id="8aaf2-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="8aaf2-112">Na caixa de diálogo de confirmação que aparece, selecione **OK**.</span><span class="sxs-lookup"><span data-stu-id="8aaf2-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="8aaf2-113">Em um navegador da web, localizar o site raiz da coleção do site, e, em seguida, acessar **site Configurações Características** \> **de coleta do site.**</span><span class="sxs-lookup"><span data-stu-id="8aaf2-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="8aaf2-114">Alternar o recurso de fluxos de **trabalho:**</span><span class="sxs-lookup"><span data-stu-id="8aaf2-114">Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="8aaf2-115">· Se o recurso for *ativado,* clique **em desativar** e, em seguida, clique **em Ativar.**</span><span class="sxs-lookup"><span data-stu-id="8aaf2-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="8aaf2-116">· Se o recurso for *desativado,* clique **em Ativar.**</span><span class="sxs-lookup"><span data-stu-id="8aaf2-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="8aaf2-117">Para mais informações, consulte o seguinte [artigo.](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)</span><span class="sxs-lookup"><span data-stu-id="8aaf2-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

