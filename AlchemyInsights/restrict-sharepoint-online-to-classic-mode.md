---
title: Restringir o SharePoint Online ao modo clássico
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 1887bf64df98bf90a1902250633d5774178dfa2f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751433"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a>Restringir o SharePoint Online ao modo clássico

Algumas organizações ainda requerem a experiência do modo Clássico. Embora não existam planos para remover o modo clássico a nível granular, já não é possível restringir toda uma organização (inquilino) ao modo clássico para listas e bibliotecas.

O administrador terá as seguintes opções para gerir listas individuais e bibliotecas em modo clássico utilizando interruptores de opt-out granular que fornecemos nos seguintes níveis:

- coleção de site
- site
- lista
- biblioteca

Além disso, as listas que usam certas funcionalidades e personalizações que não são suportadas pelo moderno ainda serão automaticamente mudadas para o modo clássico.

A partir de 1 de abril de 2019, o processo de desativação do nível de inquilino opta por sair da lista moderna e as bibliotecas vão começar e continuar até 31 de maio de 2019.  As listas e bibliotecas que estão em modo clássico como resultado do opt-out do inquilino serão automaticamente transferidas para modernas.

Se necessitar de modo clássico, consulte mais informações [aqui](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) e instruções PnP Powershell [aqui](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) que descrevem opções e ferramentas que pode usar hoje para usar a experiência clássica do modo.
