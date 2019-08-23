---
title: Restringir SharePoint Online para o modo clássico
ms.author: kirks
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
ms.openlocfilehash: e7ecfd8c2f1a532355bfb8c2c0a846fc0d6e88b1
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551570"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a>Restringir SharePoint Online para o modo clássico

Algumas organizações necessitam da experiência de modo clássico. Enquanto não existem planos para remover de modo clássico a um nível granular, já não é possível restringir toda uma organização (tenant) para o modo clássico para listas e bibliotecas.

O administrador terá as seguintes opções para gerir listas e bibliotecas na utilizando parâmetros de cancelamento granulares que fornecemos aos seguintes níveis de modo clássico individuais:

- colecção de sites
- site
- lista
- biblioteca

Além disso, listas utilizam determinadas funcionalidades e personalizações que não são suportadas pelo moderno serão ainda ser mudadas automaticamente para o modo clássico.

Início de Abril de 1 de Maio de 2019, o processo para desactivar o nível de Tenants activamente por não lista moderna e bibliotecas inicia e continue a 31 de Maio de 2019.  As listas e bibliotecas que se encontram no modo clássico na sequência de Tenants opt-out serão automaticamente transferidas para modernas.

Se necessitar de modo clássico mais informações, consulte [aqui](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) e instruções de PnP Powershell [aqui](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) que descreve as opções e ferramentas que pode utilizar hoje para utilizarem a experiência de modo clássico.
