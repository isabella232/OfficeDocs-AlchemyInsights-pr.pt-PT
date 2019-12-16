---
title: Restringir sharepoint on-line para o modo clássico
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: b58a1c3fc331c739080542917d8945c090ec0d94
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40048771"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a>Restringir sharepoint on-line para o modo clássico

Algumas organizações ainda exigem a experiência do modo Clássico. Embora não existam planos para remover o modo clássico em um nível granular, não é mais possível restringir toda uma organização (inquilino) ao modo clássico para listas e bibliotecas.

O administrador terá as seguintes opções para gerenciar listas individuais e bibliotecas no modo clássico usando interruptores de opt-out granulares que fornecemos nos seguintes níveis:

- coleção do site
- Site
- Lista
- Biblioteca

Além disso, as listas que usam determinados recursos e personalizações que não são suportadas pelo moderno ainda serão automaticamente alteradas para o modo clássico.

A partir de 1º de abril de 2019, o processo para desativar o nível do locatário desativará a lista moderna e as bibliotecas começarão e continuarão até 31 de maio de 2019.  As listas e bibliotecas que estão em modo clássico, como resultado do inquilino opt-out será automaticamente deslocado para moderno.

Se você precisar de modo clássico, consulte mais informações [aqui](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) e a instrução PnP Powershell [aqui](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) que descreva opções e ferramentas que você pode usar hoje para usar a experiência clássica do modo.
