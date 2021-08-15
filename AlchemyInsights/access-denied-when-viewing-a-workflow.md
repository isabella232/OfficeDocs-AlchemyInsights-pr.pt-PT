---
title: Access denied when viewing a Workflow
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 2b076ec5dca070555ce51b88631fb6bd619ed9269e59ccc799b23b8b95547c16
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53955212"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Access denied when viewing a Workflow

Os Fluxos de Trabalho do SharePoint 2013 que tentem enviar um e-mail para um grupo do SharePoint podem falhar com uma mensagem de erro "Acesso Negado" se a associação do grupo do SharePoint não estiver definida para Todos.
  
 **Para resolver este problema, eis os seguintes passos:**
  
 1. Permitir que todos vejam os membros do grupo do SharePoint.
  
 2. Remova o grupo do SharePoint da linha Para ou CC do e-mail.
  
 3. Adicione explicitamente os utilizadores à linha Para ou CC se a visibilidade da associação não puder ser alterada para o grupo do SharePoint.
  
Para ver mais detalhes, consulte HTTP Não autorizado para [/_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  