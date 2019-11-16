---
title: Acesso negado ao visualizar um fluxo de trabalho
ms.author: pebaum
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 4ca65583fbd98867026e9e3cc8f36fe38798aa85
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/15/2019
ms.locfileid: "36747759"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Acesso negado ao visualizar um fluxo de trabalho

Fluxos de trabalho do SharePoint 2013 que tentam enviar um e-mail para um grupo SharePoint podem falhar com uma mensagem de erro "Access Denied" se a associação do grupo SharePoint não for definida para todos.
  
 **Para resolver esse problema, faça essas etapas:**
  
 1. Permita que todos vejam os membros do grupo SharePoint.
  
 2. Retire o grupo SharePoint da linha To ou CC do e-mail.
  
 3. Adicione explicitamente os usuários à linha To ou CC se a visibilidade da associação não puder ser alterada para o grupo SharePoint.
  
Para ver mais detalhes, consulte HTTP [Não autorizado a /_vti_bin/client.svc/sp.utilities.utility.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  