---
title: Site moderno como o local de raiz
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 86ff5f7fbaed62de9047006bf4ba4d2db2be3def
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666881"
---
# <a name="modern-site-as-root-site"></a>Site moderno como site de raiz

Começamos a lançar uma nova funcionalidade que lhe permitirá [trocar o seu site clássico com um site moderno.](https://docs.microsoft.com/sharepoint/modern-root-site) Utilize [invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) para trocar a localização de um site por outro site enquanto arquiva o site original. Disponível para o Site de Equipa (não ligado a um grupo) e site de comunicação.

>[!Important]
> Não elimine o seu site de raiz clássico para criar um Site de Comunicação moderno. Isto não é suportado pela Microsoft. A eliminação do site raiz tornará todos os sites SharePoint da sua organização inacessíveis a todos os utilizadores, até que você restaure o site ou crie um novo site no mesmo URL. Vamos comunicar esta funcionalidade através do centro de mensagens. Deve esperar que a funcionalidade seja ligada ao seu inquilino em breve.

## <a name="known-issues-with-swapping-sites"></a>Problemas conhecidos com sites de troca
- O local alvo pode devolver um erro "não encontrado" (HTTP 404) por um curto período de tempo.
- O conteúdo terá de ser recrawlado para atualizar o índice de pesquisa. Não é necessário um passo manual aqui, isto será feito automaticamente.
- Qualquer coisa dependente de ligações "estáticas" (como ficheiros File Sync e OneNote) terá de ser corrigida manualmente.
- Os sites do Project Server podem ter de ser validados para garantir que ainda estão corretamente associados. 
