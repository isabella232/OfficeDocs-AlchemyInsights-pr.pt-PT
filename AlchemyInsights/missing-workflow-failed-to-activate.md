---
title: Falha ao Ativar do Fluxo de Trabalho em Falta
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: d703e87f355f05bf4a1d71e5daddce96db988380bb48accc81c95f1ba91fbb2b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54065439"
---
# <a name="missing-workflow-failed-to-activate"></a>Falha ao Ativar do Fluxo de Trabalho em Falta

Numa coleção de site do Microsoft SharePoint, não pode adicionar um fluxo de trabalho reutilizável globalmente (como "Aprovação - SharePoint 2010") a uma lista ou biblioteca.
  
Para resolver este problema, siga estes passos: 
  
1. Abra o site raiz da coleção de sites no SharePoint Designer 2013.
  
2. Em **Objetos de Site**, **selecione Fluxos de Trabalho**. 
  
3. Na secção **Novo do** grupo **Fluxos de Trabalho,** selecione Fluxo de Trabalho **Reutilizável.** 
  
4. No formulário **Criar Fluxo de Trabalho Reutilizável,** introduza o nome ** *Repair2010* **. Em **Tipo de Plataforma,** clique em **Fluxo de Trabalho do SharePoint 2010 e,** em seguida, clique **em OK.** 
  
1. Na secção **Guardar do** fita fluxo **de trabalho,** selecione **Publicar**. 
  
2. Na secção **Gerir do** grupo Fluxo **de Trabalho,** selecione **Publicar Globalmente.** Na caixa de diálogo de confirmação que é exibida, **selecione OK.** 
  
3. Num browser, localize o site raiz da coleção de sites e, em seguida, aceda a Funcionalidades da **Coleção Definições** \> **Sites.** Em seguida, ativa a funcionalidade **Fluxos de** Trabalho: 
  
· Se a funcionalidade estiver *Ativada,* clique em **Desativar e, em seguida,** clique em Ativar.  
  
· Se a funcionalidade estiver *Desativada, clique* em Ativar .  
  
Para obter mais informações, consulte o seguinte [artigo.](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)
  

