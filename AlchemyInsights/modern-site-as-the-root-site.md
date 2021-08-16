---
title: Site moderno como o site raiz
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
ms.openlocfilehash: b42cf276a76547584c8cfd87b5a28f31d51ea7f8ca56621b22aeef01e4613ce6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54000403"
---
# <a name="modern-site-as-root-site"></a>Site moderno como site raiz

Ainda começámos a lançamento de uma nova funcionalidade que lhe permitirá trocar o site raiz do [seu site clássico por um site moderno.](https://docs.microsoft.com/sharepoint/modern-root-site) Utilize [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) para trocar a localização de um site com outro site enquanto arquiva o site original. Disponível para o Site de Equipa (não ligado a um grupo) e o Site de Comunicação.

>[!Important]
> Não elimine o seu site raiz clássico para criar um Site de Comunicação moderno. Isto não é suportado pela Microsoft. Eliminar o site raiz tornará todos os sites do SharePoint na sua organização inacessíveis a todos os utilizadores até restaurar o site ou criar um novo site no mesmo URL. Iremos comunicar esta funcionalidade através do centro de mensagens. Deve esperar que a funcionalidade esteja ativada no seu inquilino em breve.

## <a name="known-issues-with-swapping-sites"></a>Problemas conhecidos com a troca de sites
- O site de destino poderá devolver um erro "não encontrado" (HTTP 404) por um curto período de tempo.
- O conteúdo terá de ser recriado para atualizar o índice de pesquisa. Não é necessário seguir passos manuais aqui. Este passo será realizado automaticamente.
- Tudo o que depender de ligações "estáticas" (como a Sincronização de Ficheiros e OneNote ficheiros) terá de ser corrigido manualmente.
- Project Os sites de servidor poderão ter de ser validados para garantir que ainda estão associados corretamente. 
