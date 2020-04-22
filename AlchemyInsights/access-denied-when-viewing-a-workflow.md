---
title: Acesso negado ao ver um Fluxo de Trabalho
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: c576bf88225582f2577e0b59506a7482cf9f38d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687341"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Acesso negado ao ver um Fluxo de Trabalho

O SharePoint 2013 Workflows que tentam enviar um e-mail para um grupo SharePoint pode falhar com uma mensagem de erro "Access Denied" se a adesão ao grupo SharePoint não estiver definida para todos.
  
 **Para resolver esta questão, faça estes passos:**
  
 1. Permita que todos vejam os membros do grupo SharePoint.
  
 2. Remova o grupo SharePoint da linha To ou CC do e-mail.
  
 3. Adicione explicitamente os utilizadores à linha To ou CC se a visibilidade da adesão não puder ser alterada para o grupo SharePoint.
  
Para ver mais detalhes consulte [http Unauthorized para /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  