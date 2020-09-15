---
title: Acesso negado ao visualizar um Fluxo de Trabalho
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 710775e8b2dee98969df7a4c8410a3e61181aaf6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688813"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Acesso negado ao visualizar um Fluxo de Trabalho

Fluxos de trabalho sharePoint 2013 que tentam enviar um e-mail para um grupo SharePoint podem falhar com uma mensagem de erro "Access Denied" se a adesão do grupo SharePoint não for definida para Todos.
  
 **Para resolver esta questão, faça estes passos:**
  
 1. Permitir que todos vejam os membros do grupo SharePoint.
  
 2. Remova o grupo SharePoint da linha To ou CC do e-mail.
  
 3. Adicione explicitamente os utilizadores à linha To ou CC se a visibilidade da adesão não puder ser alterada para o grupo SharePoint.
  
Para ver mais detalhes consulte [HTTP Não Autorizado para /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  