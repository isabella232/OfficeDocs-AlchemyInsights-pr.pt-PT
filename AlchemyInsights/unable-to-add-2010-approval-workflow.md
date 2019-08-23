---
title: Não é possível adicionar o fluxo de trabalho de aprovação de 2010
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: 1f564c5d1e689dcf41b22fab5a05ab1b488c2b0b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36558628"
---
# <a name="unable-to-add-2010-approval-workflow"></a>Não é possível adicionar o fluxo de trabalho de aprovação de 2010

Uma colecção de sites do Microsoft SharePoint, não é possível adicionar um fluxo de trabalho reutilizável globalmente (por exemplo, "aprovação - SharePoint 2010") para uma lista ou biblioteca.
  
Para resolver este problema, siga estes passos: 
  
1. Abra o Web site de raiz da colecção de sites no SharePoint Designer 2013.
  
2. Em **Objectos de Site**, seleccione os **fluxos de trabalho**. 
  
3. Na secção **Novo** friso **fluxos de trabalho** , seleccione o **Fluxo de trabalho reutilizável**. 
  
4. No formulário **Criar fluxo de trabalho reutilizável** , introduza o nome * * *Repair2010* * *. Para **Tipo de plataforma**, faça clique sobre **o fluxo de trabalho do SharePoint 2010**e, em seguida, clique em **OK**. 
  
1. Na secção **Guardar** do Friso de **fluxo de trabalho** , seleccione **Publicar**. 
  
2. Na secção **Gerir** o Friso de **fluxo de trabalho** , seleccione **Publicar globalmente**. Na caixa de diálogo de confirmação que aparece, seleccione **' OK '**. 
  
3. Num web browser, localize o Web site de raiz da colecção de sites e, em seguida, aceder a **Definições do Site** \> **Funcionalidades de colecção de sites**. Activar/desactivar a funcionalidade de **fluxos de trabalho** : 
  
· Se a funcionalidade estiver *activada* , clique em **desativar** e, em seguida, clique em **Activar**. 
  
· Se a funcionalidade de *Deactivated* , clique em **Activar**. 
  
Para obter mais informações, consulte o seguinte [artigo](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

