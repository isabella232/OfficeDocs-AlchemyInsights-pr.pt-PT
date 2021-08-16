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
ms.openlocfilehash: f99bb449b542760c6c8d51ee399c774fbe36e3f7f40520b5eb23f39d9d7c08dd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53968388"
---
# <a name="changing-ews-throttling-settings"></a>Alterar as definições de limitação do EWS

Execute o nosso teste automatizado que lhe permite modificar a política de limitação do EWS durante o período da sua migração. Tenha em atenção que, mesmo após esta execução, a importação do EWS permanecerá limitada a 150MB por 5 minutos por caixa de correio. Para obter velocidades de débito mais elevadas durante a migração, efetue a migração de mais utilizadores em simultâneo.

Tenha em atenção que as alterações da política de limitação do EWS não produz efeito nos seguintes tipos de migração (através das ferramentas da Microsoft): Híbrida, Migração de Transferência/Faseada (RPC/HTTP), IMAP, G Suite, Pasta Pública ou Serviço de Importação de Ficheiros PST.