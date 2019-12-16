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
# <a name="unable-to-add-2010-approval-workflow"></a>Incapaz de adicionar o fluxo de trabalho de aprovação de 2010

Em uma coleção de sites do Microsoft SharePoint, você não pode adicionar um fluxo de trabalho globalmente reutilizável (como "Aprovação - SharePoint 2010") a uma lista ou biblioteca.
  
Para resolver este problema, siga estas etapas: 
  
1. Abra o site raiz da coleção do site em SharePoint Designer 2013.
  
2. **objetos do site,** selecione fluxos de **trabalho.** 
  
3. Na **nova** seção da fita **workflows,** selecione fluxo de **trabalho reutilizável.** 
  
4. No formulário criar fluxo de **trabalho reutilizável,** digite o nome ** *Repair2010* **. Para **o tipo de plataforma,** clique no fluxo de trabalho **sharepoint 2010**e, em seguida, clique na **OK.** 
  
1. Na seção **Save** da fita **workflow,** **selecione Publicar**. 
  
2. Na seção **gerenciar** da fita **workflow,** selecione **Publicar Globalmente**. Na caixa de diálogo de confirmação que aparece, selecione **OK**. 
  
3. Em um navegador da web, localizar o site raiz da coleção do site, e, em seguida, acessar **site Configurações Características** \> **de coleta do site.** Alternar o recurso de fluxos de **trabalho:** 
  
· Se o recurso for *ativado,* clique **em desativar** e, em seguida, clique **em Ativar.** 
  
· Se o recurso for *desativado,* clique **em Ativar.** 
  
Para mais informações, consulte o seguinte [artigo.](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)
  

