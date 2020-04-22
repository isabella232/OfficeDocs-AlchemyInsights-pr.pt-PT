---
title: Local moderno como o local de raiz
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 0388f95e2b7815dcbbb6aca200f44e55e9c5724f
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713802"
---
# <a name="modern-site-as-root-site"></a>Local moderno como local de raiz

Começamos a lançar uma nova funcionalidade que lhe permitirá [trocar o seu site clássico com um site moderno.](https://docs.microsoft.com/sharepoint/modern-root-site) Utilize o [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) para trocar a localização de um site por outro site enquanto arquiva o site original. Disponível tanto para o Site da Equipa (não ligado a um grupo) como para o Site de Comunicação.

>[!Important]
> Não elimine o seu site de raiz clássico para criar um site de comunicação moderno. Isto não é suportado pela Microsoft. A eliminação do site raiz tornará inacessíveis todos os sites do SharePoint na sua organização a todos os utilizadores, até que restaure o site ou crie um novo site no mesmo URL. Vamos comunicar esta funcionalidade através do centro de mensagens. Deve esperar que a funcionalidade seja ligada no seu inquilino em breve.

## <a name="known-issues-with-swapping-sites"></a>Questões conhecidas com sites de troca
- O local-alvo pode devolver um erro "não encontrado" (HTTP 404) por um curto período de tempo.
- O conteúdo terá de ser reescrito para atualizar o índice de pesquisa. Não é necessário um passo manual aqui, isto será feito automaticamente.
- Qualquer coisa dependente de links "estáticos" (como ficheiros Sync e OneNote) terá de ser corrigido manualmente.
- Os sites do Project Server podem ter de ser validados para garantir que ainda estão corretamente associados. 
