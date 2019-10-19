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
# <a name="missing-workflow-failed-to-activate"></a>Falha no fluxo de trabalho ausente para ativar

Em um conjunto de sites do Microsoft SharePoint, você não pode adicionar um fluxo de trabalho globalmente reutilizável (como "aprovação-SharePoint 2010") a uma lista ou biblioteca.
  
Para resolver este problema, siga estes passos: 
  
1. Abra o site raiz do conjunto de sites no SharePoint Designer 2013.
  
2. Em **objetos do site**, selecione **fluxos de trabalho**. 
  
3. Na **nova** seção da faixa de opções **fluxos de trabalho** , selecione fluxo de **trabalho reutilizável**. 
  
4. No formulário **criar fluxo de trabalho reutilizável** , digite o nome * * *Repair2010* * *. Para **tipo de plataforma**, clique em **SharePoint 2010 Workflow**e, em seguida, clique em **OK**. 
  
1. Na seção **salvar** da faixa de opções de **fluxo de trabalho** , selecione **publicar**. 
  
2. Na seção **gerenciar** da faixa de opções **fluxo de trabalho** , selecione **publicar globalmente**. Na caixa de diálogo de confirmação que aparece, selecione **OK**. 
  
3. Em um navegador da Web, localize o site raiz do conjunto de sites e, em seguida, acesse **recursos de conjunto**de sites de **configurações** \> do site. Em seguida, alterne o recurso de **fluxos de trabalho** : 
  
· Se o recurso estiver *ativado* , clique em **desativar** e, em seguida, clique em **Ativar**. 
  
· Se o recurso estiver *desativado* , clique em **Ativar**. 
  
Para obter mais informações, consulte o seguinte [artigo](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

