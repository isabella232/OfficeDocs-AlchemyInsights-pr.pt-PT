---
title: Não é possível adicionar fluxo de trabalho de aprovação de 2010
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: aa61f1615b60d27cffad15f02f6ce5dbac1b607f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47699746"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="757fd-102">Não é possível adicionar fluxo de trabalho de aprovação de 2010</span><span class="sxs-lookup"><span data-stu-id="757fd-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="757fd-103">Numa coleção de sites do Microsoft SharePoint, não é possível adicionar um fluxo de trabalho globalmente reutilizável (como "Approval - SharePoint 2010") a uma lista ou biblioteca.</span><span class="sxs-lookup"><span data-stu-id="757fd-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="757fd-104">Para resolver esta questão, siga estes passos:</span><span class="sxs-lookup"><span data-stu-id="757fd-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="757fd-105">Abra o site de raiz da coleção do site no SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="757fd-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="757fd-106">Em **Objetos do Local,** selecione **Fluxos de Trabalho.**</span><span class="sxs-lookup"><span data-stu-id="757fd-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="757fd-107">Na **nova** secção da fita **Workflows,** selecione **Fluxo de Trabalho Reutilizável**.</span><span class="sxs-lookup"><span data-stu-id="757fd-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="757fd-108">No formulário **De Fluxo de Trabalho Reutilizável, insira** o nome \*\* *Reparação2010* \*\*.</span><span class="sxs-lookup"><span data-stu-id="757fd-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="757fd-109">Para **o Tipo de Plataforma**, clique no Fluxo de Trabalho do **SharePoint 2010**e, em seguida, clique em **OK**.</span><span class="sxs-lookup"><span data-stu-id="757fd-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="757fd-110">Na secção **Guardar** a fita **Workflow,** selecione **Publicar**.</span><span class="sxs-lookup"><span data-stu-id="757fd-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="757fd-111">Na secção **Gerir** a fita **Workflow,** selecione **Publicar Globalmente**.</span><span class="sxs-lookup"><span data-stu-id="757fd-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="757fd-112">Na caixa de diálogo de confirmação que aparece, selecione **OK**.</span><span class="sxs-lookup"><span data-stu-id="757fd-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="757fd-113">Num navegador web, localize o site raiz da **Site Settings** coleção do site e, em seguida, aceda às \> **Funcionalidades de Recolha do Site**.</span><span class="sxs-lookup"><span data-stu-id="757fd-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="757fd-114">Alternar a função **Fluxos de Trabalho:**</span><span class="sxs-lookup"><span data-stu-id="757fd-114">Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="757fd-115">· Se a função estiver  *Ativada,*  clique em **Desativar e,** em seguida, clique em **Ativar**.</span><span class="sxs-lookup"><span data-stu-id="757fd-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="757fd-116">· Se a função estiver  *desativada,*  clique em **Ativar**.</span><span class="sxs-lookup"><span data-stu-id="757fd-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="757fd-117">Para mais informações, consulte o [seguinte artigo.](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)</span><span class="sxs-lookup"><span data-stu-id="757fd-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

