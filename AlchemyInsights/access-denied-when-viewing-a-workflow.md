---
title: Acesso negado quando estiver a ver um fluxo de trabalho
ms.author: kirks
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: b7a3805d30cac44781adbbb00c0f0ed3496ff17b
ms.sourcegitcommit: a9be2e396022382e92cf40c0d0d82f2f59c2e259
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/12/2019
ms.locfileid: "34883602"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Acesso negado quando estiver a ver um fluxo de trabalho

Fluxos de trabalho do SharePoint 2013 que tentar enviar mensagens de correio electrónico a um grupo SharePoint pode falhar com uma mensagem de erro "Acesso negado" se os membros do grupo do SharePoint não está definido para todos os utilizadores.
  
 **Para resolver este problema, execute estes passos:**
  
 1. Permitir que todas as pessoas ver os membros do grupo do SharePoint.
  
 2. Remova o grupo do SharePoint para ou CC linha da mensagem de correio electrónico.
  
 3. Adicionar explicitamente os utilizadores para ou CC linha se não pode ser alterada a visibilidade de membros de grupo do SharePoint.
  
Para ver mais detalhes consulte [HTTP não autorizado para /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  