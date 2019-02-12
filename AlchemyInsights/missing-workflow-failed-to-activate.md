---
title: Falta o fluxo de trabalho não conseguiu activar
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: ce088227a3206fa05b99331fdb022fbe4886203f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/12/2019
ms.locfileid: "29917579"
---
# <a name="missing-workflow-failed-to-activate"></a>Falta o fluxo de trabalho não conseguiu activar

Uma colecção de sites do Microsoft SharePoint, não é possível adicionar um fluxo de trabalho reutilizável globalmente (por exemplo, "aprovação - SharePoint 2010") para uma lista ou biblioteca.
  
Para resolver este problema, siga estes passos: 
  
1. Abra o Web site de raiz da colecção de sites no SharePoint Designer 2013.
  
2. Em **Objectos de Site**, seleccione os **fluxos de trabalho**. 
  
3. Na secção **Novo** friso **fluxos de trabalho** , seleccione o **Fluxo de trabalho reutilizável**. 
  
4. No formulário **Criar fluxo de trabalho reutilizável** , introduza o nome * * *Repair2010* * *. Para **Tipo de plataforma**, faça clique sobre **o fluxo de trabalho do SharePoint 2010**e, em seguida, clique em **OK**. 
  
1. Na secção **Guardar** do Friso de **fluxo de trabalho** , seleccione **Publicar**. 
  
2. Na secção **Gerir** o Friso de **fluxo de trabalho** , seleccione **Publicar globalmente**. Na caixa de diálogo de confirmação que aparece, seleccione **' OK '**. 
  
3. Num web browser, localize o Web site de raiz da colecção de sites e, em seguida, aceder a **Definições do Site** \> **Funcionalidades de colecção de sites**. Em seguida, activar/desactivar a funcionalidade de **fluxos de trabalho** : 
  
· Se a funcionalidade estiver *activada* , clique em **desativar** e, em seguida, clique em **Activar**. 
  
· Se a funcionalidade de *Deactivated* , clique em **Activar**. 
  
Para obter mais informações, consulte o seguinte [artigo](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

