---
title: Fluxo de trabalho desaparecido falhou em ativar
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 604dc770c5c14ded6a8de1cec9e311b03b69f094
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667097"
---
# <a name="missing-workflow-failed-to-activate"></a>Fluxo de trabalho desaparecido falhou em ativar

Numa coleção de sites do Microsoft SharePoint, não é possível adicionar um fluxo de trabalho globalmente reutilizável (como "Approval - SharePoint 2010") a uma lista ou biblioteca.
  
Para resolver esta questão, siga estes passos: 
  
1. Abra o site de raiz da coleção do site no SharePoint Designer 2013.
  
2. Em **Objetos do Local,** selecione **Fluxos de Trabalho.** 
  
3. Na **nova** secção da fita **Workflows,** selecione **Fluxo de Trabalho Reutilizável**. 
  
4. No formulário **De Fluxo de Trabalho Reutilizável, insira** o nome ** *Reparação2010* **. Para **o Tipo de Plataforma**, clique no Fluxo de Trabalho do **SharePoint 2010**e, em seguida, clique em **OK**. 
  
1. Na secção **Guardar** a fita **Workflow,** selecione **Publicar**. 
  
2. Na secção **Gerir** a fita **Workflow,** selecione **Publicar Globalmente**. Na caixa de diálogo de confirmação que aparece, selecione **OK**. 
  
3. Num navegador web, localize o site raiz da **Site Settings** coleção do site e, em seguida, aceda às \> **Funcionalidades de Recolha do Site**. Em seguida, alternar a função **Workflows:** 
  
· Se a função estiver  *Ativada,*  clique em **Desativar e,** em seguida, clique em **Ativar**. 
  
· Se a função estiver  *desativada,*  clique em **Ativar**. 
  
Para mais informações, consulte o [seguinte artigo.](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)
  

