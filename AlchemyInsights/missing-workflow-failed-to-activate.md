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
# <a name="missing-workflow-failed-to-activate"></a>Fluxo de trabalho desaparecido falhou em ativar

Numa coleção de site do Microsoft SharePoint, não é possível adicionar um fluxo de trabalho globalmente reutilizável (como "Approval - SharePoint 2010") a uma lista ou biblioteca.
  
Para resolver esta questão, siga estes passos: 
  
1. Abra o site raiz da coleção do site no SharePoint Designer 2013.
  
2. Sob **os Objetos do Site,** selecione **Fluxos de Trabalho**. 
  
3. Na **nova** secção da fita **Workflows,** selecione Fluxos de **Trabalho Reutilizáveis**. 
  
4. No formulário **Create Reutilable Workflow,** introduza o nome ** *Repair2010* **. Para **o Tipo de Plataforma,** clique no **SharePoint 2010 Workflow**, e depois clique em **OK**. 
  
1. Na secção **Guardar** da fita **Workflow,** selecione **Publicar**. 
  
2. Na secção **Gerir** a fita **Workflow,** selecione **Publicar Globalmente**. Na caixa de diálogo de confirmação que aparece, selecione **OK**. 
  
3. Num navegador web, localize o site raiz da coleção do site e, em seguida, aceda às **Funcionalidades**de Recolha do **Site** \> . Em seguida, alternar a função **Workflows:** 
  
· Se a funcionalidade for *Ativada,* clique em **Desativar** e, em seguida, clique em **Ativar**. 
  
· Se a funcionalidade for *desativada,* clique **em Ativar**. 
  
Para mais informações, consulte o [seguinte artigo](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

