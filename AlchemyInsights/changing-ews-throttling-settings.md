---
title: Alterar as definições de limitação do EWS
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000752"
- "5653"
- "5760"
ms.openlocfilehash: 16916d5f16f763d87ce0d5ef830e741279c9f4df
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818047"
---
# <a name="changing-ews-throttling-settings"></a>Alterar as definições de limitação do EWS

Execute o nosso teste automatizado que lhe permite modificar a política de limitação do EWS durante o período da sua migração. Tenha em atenção que, mesmo após esta execução, a importação do EWS permanecerá limitada a 150MB por 5 minutos por caixa de correio. Para obter velocidades de débito mais elevadas durante a migração, efetue a migração de mais utilizadores em simultâneo.

Tenha em atenção que as alterações da política de limitação do EWS não produz efeito nos seguintes tipos de migração (através das ferramentas da Microsoft): Híbrida, Migração de Transferência/Faseada (RPC/HTTP), IMAP, G Suite, Pasta Pública ou Serviço de Importação de Ficheiros PST.