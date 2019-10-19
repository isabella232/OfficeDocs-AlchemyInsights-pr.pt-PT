---
title: Restringir o SharePoint Online ao modo clássico
ms.author: pebaum
author: Techwriter40
ms.date: 3/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 18d263593d99f24c3020336ae601df14dbbf5411
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/18/2019
ms.locfileid: "36752079"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a>Restringir o SharePoint Online ao modo clássico

Algumas organizações ainda exigem a experiência de modo clássico. Embora não haja planos para remover o modo clássico em um nível granular, não é mais possível restringir uma organização inteira (locatário) para o modo clássico para listas e bibliotecas.

O administrador terá as seguintes opções para gerenciar listas e bibliotecas individuais no modo clássico usando switches de desativação granular que fornecemos nos seguintes níveis:

- coleção de sites
- Site
- Lista
- Biblioteca

Além disso, as listas que usam determinados recursos e personalizações que não são suportadas pelo moderno ainda serão automaticamente alternadas para o modo clássico.

A partir de 1 de abril de 2019, o processo para desativar o nível de inquilino opt out da lista moderna e bibliotecas irá iniciar e continuar até 31 de maio de 2019.  As listas e bibliotecas que estão no modo clássico como resultado da desativação do locatário serão automaticamente deslocadas para o moderno.

Se você precisar de modo clássico, consulte mais informações [aqui](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) e instruções do PowerShell PNP [aqui](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) que descreve as opções e ferramentas que você pode usar hoje para usar a experiência de modo clássico.
