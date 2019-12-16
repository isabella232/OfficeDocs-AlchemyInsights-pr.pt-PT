---
title: Local moderno como o local da raiz
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 2e2bb02b9dbaf7f8ede0b4c5ba8c8f29453309cb
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40054713"
---
# <a name="modern-site-as-root-site"></a>Local moderno como o local da raiz

Começamos a lançar um novo recurso que lhe permitirá [trocar seu site clássico com um site moderno.](https://docs.microsoft.com/sharepoint/modern-root-site) Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) para trocar a localização de um site com outro site enquanto arquiva o site original. Disponível para o Site da Equipe (não conectado a um grupo) e ao Site de Comunicação.

>[!Important]
> Não exclua seu site clássico de raiz para criar um site de comunicação moderno. Isso não é suportado pela Microsoft. A exclusão do site raiz tornará todos os sites do SharePoint em sua organização inacessíveis a todos os usuários, até que você restaure o site ou crie um novo site na mesma URL. Estaremos comunicando esse recurso através do centro de mensagens. Você deve esperar que o recurso seja ativado em seu inquilino em breve.

## <a name="known-issues-with-swapping-sites"></a>Problemas conhecidos com a troca de sites
- O site-alvo pode retornar um erro "não encontrado" (HTTP 404) por um curto período de tempo.
- O conteúdo precisará ser rerabiscado para atualizar o índice de pesquisa. Não há nenhuma etapa manual exigida aqui, esta será feita automaticamente.
- Qualquer coisa dependente de links "estáticos" (como arquivos File Sync e OneNote) precisará ser corrigido manualmente.
- Os sites do Servidor do Projeto podem precisar ser validados para garantir que eles ainda estejam associados corretamente. 
