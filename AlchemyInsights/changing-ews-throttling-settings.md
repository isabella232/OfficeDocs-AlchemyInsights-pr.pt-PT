---
title: Alterar as definições de limitação do EWS
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 4f0bea884153dc1ed8699ce12e0d017d18f5e57c
ms.sourcegitcommit: 53e5caab697ebfb434ccef3ef98b8f2bee579b41
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/02/2021
ms.locfileid: "50075908"
---
# <a name="changing-ews-throttling-settings"></a>Alterar as definições de limitação do EWS

Execute o nosso teste automatizado que lhe permite modificar a política de limitação do EWS durante o período da sua migração. Tenha em atenção que, mesmo após esta execução, a importação do EWS permanecerá limitada a 150MB por 5 minutos por caixa de correio. Para obter velocidades de débito mais elevadas durante a migração, efetue a migração de mais utilizadores em simultâneo.

Tenha em atenção que as alterações da política de limitação do EWS não produz efeito nos seguintes tipos de migração (através das ferramentas da Microsoft): Híbrida, Migração de Transferência/Faseada (RPC/HTTP), IMAP, G Suite, Pasta Pública ou Serviço de Importação de Ficheiros PST.